# Domain Model
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


## Classes
### AdvisorInformation
- Retrieves the advisor information and matches it to their clients
### ClientInformation
- Retrieves the client information and matches it to their portfolio
### Controller
- Processes requests between all the other aspects of the domain
### API
- Processes requests between the Controller and the Llama AI
### FrontEnd
- An admin terminal to help test the API
### EmailClass
- Summarizes the information from the AI prompt and then sends it as an email
### Trigger
- Checks if new quarterly statements are out
### Llama 
- Generative AI tool
### Document
- Collection of portfolio related assets that pertain to the client
### Stock
- Financial Asset
### Mutual Fund
- Collection of stocks/ bonds
