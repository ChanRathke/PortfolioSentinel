This document will be like a user manual for your end users that shows how to use the various features of your software with pictures step by step.
Assume your software is available to the end-user in some form through a URL or installation of the binary.

Testing criteria for this document:
  A regular user should be able to use the features of your running project by just following this document.


# Running the Program

## Beginning in the Command Line
The user will begin in the terminal of the program. The user must first start the backend, so to change directorys, use: `cd Backend`

Next, the user will simply run `python fetch_calls.py`

Now the user should open a new, second terminal and change the directory to be in the Frontend folder by using: `cd Frontend`

Then, simply input the following commands: 
  `npm install --legacy-peer-deps`
  `npm run dev`

The user should then open the browser by either clicking on the link provided by "Local:" or entering it into your browser manually.

The link should look like this `http://localhost:5173/`

![npmRunDev](https://github.com/user-attachments/assets/5c5b3c4d-c8d4-4101-a927-a5a56ce22f82)

## Using Docker
Another method to start the program is to use docker. With this method, the user simply inputs `start start.bat`

This will run both the Frontend and Backend for the user and they can hit the link from the frontend terminal when it presents itself.

Just like the previous method, the link should look like `http://localhost:5173/`



## User Interface
The user should then see the interface of Portfolio Sentinel.

The user can see a search bar which will populate as the user types into it.
![first](https://github.com/user-attachments/assets/bd2e7964-5783-4699-a4e6-00bda4864f29)


Once the user has selected a stock, they can select a question from the dropdown menu for a number of different summaries that are provided.

![second](https://github.com/user-attachments/assets/8906e6f6-8b05-40ee-ac2b-738bfccd4253)


Finally, the user needs to simply select the "Get Summary" button to see the information that the AI has output. They can also cancel the task if they wish.

![third](https://github.com/user-attachments/assets/0b39df1d-614c-4562-a15c-718931f0cf1d)


In the next section, there is a "Portfolio Manager" to help the user create and analyze portfolios.

The first screenshot shows the user having selected a TSLA stock where they will also type in the allocation of the stock in their portfolio. 

![fourth](https://github.com/user-attachments/assets/25cdd92b-e847-4f1e-bad8-e52874a76bc3)


After the stocks are added to the portfolio with the button, they should be present on the screen along with their allocations. 

Now the user simply clicks the "Analyze Portfolio" button to wait for a result from the AI. 

![fifth](https://github.com/user-attachments/assets/4a232adb-329a-41b6-b41f-581cdc052f89)








