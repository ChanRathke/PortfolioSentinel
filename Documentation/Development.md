# Development

## Tech Aspects
- Vue
- Python
- BitBucket

## IDE
- Visual Studio Code
- Gemini AI

# Preparing to Run

## Install Prerequisites
- Install [.NET (v8.0)](https://dotnet.microsoft.com/en-us/download)
  
  ![net](https://github.com/user-attachments/assets/aca0acd0-f5f8-4872-bd8f-bec6b8dc5461)

- Install the latest version of [Python](https://www.python.org/downloads/). (Tested on 3.13.0)

  ![image](https://github.com/user-attachments/assets/bfaaba9f-2d43-4845-a394-9abe2bf04fe6)

  

## Create a Clone Repository
- If you will contribute, fork this repository first and clone your copies.
- Run `git clone https://bitbucket.org/accutechcapstone/bsu.portfoliosentinel.git` to retrieve the repo and save it where you'd like

## Preparing to Run the Program
- Open the project either through the command line or opening the folder 
- Open the terminal of the project and run the following commands:
    - `pip install -U google-generativeai`
    - `npm install`
    - `npm install axios`
    - `npm install flask`
    - `npm install vite`
## To Run the Program
- Open the terminal
- Change the directory into the Frontend folder: `cd test-project`
- Run the following code: `npm run dev`
- Open the browser by either clicking on the link provided by "Local:" or entering it into your browser manually
    - It should look like this: `http://localhost:5173/`
- Open a 2nd terminal
- Change the directory into the backend folder: `cd test-api`
- Run `fetch_calls.py` by doing `python fetch_calls.py`

## Replicating via Docker

Alternatively you can run the program in docker.

- Install [Docker Desktop](https://www.docker.com/products/docker-desktop)

  ![image](https://github.com/user-attachments/assets/fa05e045-3bdf-430d-a629-f8d0f1d6fc1c)
- With docker desktop running: 
  - Navigate to the clone of the repository.
  - Either in file explorer or in the command terminal, run the file labeled `start.bat`.
    - If you want to test them individually: run `backend.bat` for the backend, or `frontend.bat` for the frontend.
    - Note: These files will run the docker commands for you.
  - 2 seperate terminals will pop up, one for the front end and one for the backend.
  - To view the frontend, click on the VITE localhost link that pops up in the terminal
    - It should look like this: `http://localhost:5173/`
 
    
