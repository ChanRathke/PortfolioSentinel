## Functional Requirements
- FR1: Advisor management
        - retrieve advisor information high
        - create new advisor medium
        - delete advisor medium
        - list of clients linked to advisor high
- FR2: Client management
        - retrieve client information and link to portfolio high
        - create new clients medium
        - delete clients medium
- FR3: Document management
        - retreieve advisor email high
        - retrieve quarterly statements for client and advisor high
        - trigger when new documents are available high
- FR4: Email notification
        - retrieve advisor email medium
        - generate and send emails to advisor when new documents are available high
- FR5: API integration
        - system retrieve summary of stock information by external AI API medium
        - request from controller and fetch data high
- FR6: trigger
        - system checks for quarterly documents high
        - system initaite the process of notifying relevent parties when new document is available high
- FR7: Controller
        - system handling communication between UI, Advisor, client, and document, and API high
- FR8: frontend interface
        - frontend prompt the user for advisor and client high
        - system allowing the user to trigger document checks and sends emails through interface high
- FR9: Llama AI
        - system must integrate with llama AI to retrieve relevent stock summaries based on inputs from API medium


## Nonfunctional Requirements
- NR1: Performance
        - retrieve advisor and client information from database with no delay high
- NR2: Scalability
        - system should be able to handle a growing number of advisors and clients and documents medium
- NR3: Secuirty
        - advisor and client information to be stored and transferred securely high
- NR4: Reliablity
        - system must reliably detect ad trigger alerts for new documents high
- NR5: Usability
        - frontend interface to be intuitive for users, input for clients and advisors details and managing document triggers high
- NR6: Maintainability
        - system architecture should be modular for easy maintenance and updates to individual components like APi, EmailClass and controller medium
- NR7: Integration
        - API and controller have an effectively manage interaction with external services medium
- NR8: Data accuracy
        - system ensure accurate retrieval and representation of document, advisor, and client high




Ideas for requirements from DesignDraft:
-Default prompt for generative AI summary
-Default prompt for email
-API 
-Generative AI describes changes.
-A generative AI can describe why a change occurred in a portfolio.