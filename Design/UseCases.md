# Actors
- Client
- Advisor
- Gemini
- Email Service

# Use Cases
### UC1: Monitor Portfolio Changes
- **Primary Actors:** Client and Advisor
- Monitoring portfolio changes is a key function of the system. Clients need to be informed about the status of their investments and any changes that may impact their portfolio. On a quarterly basis, the system will check for any changes, retrieve relevant information, and email the advisor. This enables the advisor to inform the client and make the appropriate decisions.
  
  1. The system checks for changes in the portfolio quarterly
  2. The system retrieves relevant information and checks for new quarterly statements
  3. The Controller communicates with the API and Llama to create an analysis of these changes
  4. The summary is emailed to the client
- **Business Requirement:** BR1

### UC2: View Advisor's Clients
- **Primary Actors:** Advisor
- One of our requirements was to allow advisors to manage their clients and have access to their clients’ portfolio details to make informed investment decisions. This allows advisors to retrieve necessary information and data to help them stay updated and effectively manage their clients' portfolios.

  1. The advisor logs into the system using their email
  2. The advisor can view their profile and their clients' information
  3. The system retrieves and displays the client portfolio details
  4. The advisor can then use this information to inform or update the client
- **Business Requirement:** BR1

### UC3: Generate Quarterly Portfolio Summary
- **Primary Actors:** Gemini
- One of our main business requirements was generating a quarterly portfolio summary. This involves using Gemini to generate a detailed analysis of each client’s portfolio. The generated summary is then automatically sent to the advisor, allowing them to review and share the relevant information with their clients.

  1. The system triggers the quarterly summary generation
  2. The system gathers relevant market data and client portfolio details
  3. Sends the data to Gemini for analysis
  4. Gemini generates a detailed summary of the portfolio's performance
- **Business Requirement:** BR1

### UC4: Automated Emails to Advisor
- **Primary Actors:** Advisor and Email Service
- One business requirement was to automate emails to advisors to keep them informed about their clients' portfolio details. The system ensures that once the system generates the portfolio summary, an automated email is sent to the advisor with portfolio insights to allow them to communicate with their clients.

  1. The system completes quarterly portfolio analysis and generates a summary
  2. The system automatically formats the summary into an email
  3. The system uses an email service to send the summary to the advisor's registered email
  4. The advisor receives the email with the portfolio summary for their review
- **Business Requirement:** BR1
