## Functional Requirements
- FR1: Advisor management
        - retrieve advisor information (and their clients):
  - High priority
  - UC2 
- FR2: Client management
        - retrieve client information and link to portfolio:
  - High priority
  - UC1
- FR3: Document management
        - retrieve quarterly statements for client and advisor:
  - High priority
  - UC1
- FR4: Email notification
        - generate and send emails to advisor when new documents are available:
  - High priority
  - UC4
- FR5: API integration
        - system retrieve summary of stock information by external AI API:
  - Medium priority
  - UC1
- FR6: Trigger
        - system initaites the process of notifying relevent parties when new quarterly document is available:
  - High priority
  - UC4
- FR7: Controller
        - system handling communication between UI, Advisor, client, and document, and API:
  - High priority
  - UC1
- FR8: Frontend interface
        - user can select a number of stocks to gain informatiom on:
  - High priority
  - UC4
- FR9: Gemini AI
        - system must integrate with gemini AI to retrieve relevent stock summaries based on inputs from API:
  - High priority
  - UC3
- FR10: Alpha Vantage API
        - system must integrate with alpha vantage API to retrieve relevant stock/news data.
  - High priority
  - UC3     
    

## Nonfunctional Requirements
- NR1: Performance
        - retrieve advisor and client information from database with no delay
  - High
  - UC2
- NR2: Scalability
        - system should be able to handle a growing number of advisors and clients and documents
  - Medium
  - UC2
- NR3: Secuirty
        - advisor and client information to be stored and transferred securely
  - High
  - UC2
- NR4: Reliablity
        - system must reliably detect ad trigger alerts for new documents
  - High
  - UC1
- NR5: Usability
        - frontend interface to be intuitive for users, input for clients and advisors details and managing document triggers
  - High
  - UC1
- NR6: Maintainability
        - system architecture should be modular for easy maintenance and updates to individual components like API, EmailClass and controller
  - Medium
  - UC3
- NR7: Integration
        - API and controller have an effectively manage interaction with external services
  - Medium
  - UC3
- NR8: Data accuracy
        - system ensure accurate retrieval and representation of document, advisor, and client
  - High
  - UC1
