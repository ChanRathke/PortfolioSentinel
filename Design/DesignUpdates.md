##**Tech Stack:** Nothing changed from original submission.
##**Architecture:** Changed reference from LLama AI to Gemini and Alpha Vantage
## **Old:**
- ![image](https://github.com/user-attachments/assets/e0cfe58f-43b4-4d61-bd6c-e6f7b2eb47e7)
## **New:**
- ![image](https://github.com/user-attachments/assets/3c993ae7-da68-4380-8d7b-5a4fb7f7be6f)

##**Domain Model:** Editted based on instructor feedback, removing references to APIs / Controllers. 
##**Old:**
```mermaid
classDiagram
Document <|-- Controller
Controller --|> API
Document --|> Trigger
Document --|> Client
FrontEnd --|> Client
FrontEnd --|> Advisor
Advisor --|> Client
Trigger --|> Controller 
EmailClass <|-- Controller
EmailClass <|-- API
API <|--|> Llama
Document --|> Stock
Document --|> MutualFund
Mutual Fund --|> Stock
class Advisor {
      advisorName: String
      email: String
      clients: Client[]
      addClient()
      removeClient(Client)
      getEmail(): String
}
class Client {
      clientName: String
      advisor: Advisor
      portfolio: Document
      getAdvisor(): Advisor
      setAdvisor(Advisor)
      getClientPortfolio(): Document
}
class Document {
      stocks: Stock[]
      mutualFunds: MutualFund[]
      client: Client
      getStocks(): Stock[]
      getMutualFunds(): MutualFund[]
      getClient(): Client
}
class Trigger {
      checkQuarterly(Stock): Boolean
      checkQuarterly(MutualFund): Boolean
}
class FrontEnd {
      getClientInfo(): Client
      getAdvisorInfo(): Advisor
}
class API{
      getSummary(Stock)
}
class EmailClass {
      sendEmail(Advisor, String)
}
```
## **New:**
```mermaid
classDiagram
Document <|-- Client
Advisor --|> Client
Email --|> Advisor
Document --|> Stock
Document --|> MutualFund
Document --|> Email
Stock --|> Summary
MutualFund --|> Summary
Summary --|> Email
Mutual Fund <|-- Stock
class Advisor {
      id: String
      advisorName: String
      advisorEmail: String
      clients: Client[]
}
class Client {
      id: String
      clientName: String
      advisor: Advisor
      clientEmail: String
      portfolio: Document
}
class Document {
      stocks: Stock[]
      mutualFunds: MutualFund[]
      client: Client
}
class Email {
      sendEmail(Advisor, Summary)
}
class Summary {
      summary: String
      generateSummary(Stock): String
}
class MutualFund {
      name: String
      getStocks(): Stock[]
}
class Stock {
      ticker:  String
      name: String
}
```
## **Use Cases:** Replaced all references to Llama with references to Gemini / Alpha Vantage

## **Business Requirements:** Updated BR1 based on instructor feedback.
**Old:** A generative AI will summarize information and update the client based on their needs.
**New:** Keep Advisors updated on changes within their clientelles investments so that they can more easily inform their client about it.
