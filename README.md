# VigilGit

## Description
**VigilGit** is a lightweight, high-performance security microservice designed to act as an automated guardrail for your development workflow. Built with **FastAPI** and powered by Yelp’s enterprise-grade `detect-secrets` engine, VigilGit integrates seamlessly with GitHub webhooks to intercept real-time code pushes, scan payloads across multiple detection plugins, and block accidental credential leaks before they ever hit production.

## Tech Stack

* **Language:** Python 3.9+
* **Framework:** FastAPI/Uvicorn
* **Security Engine:** Yelp 'detect-secrets'
* **Integration:** GitHub Apps and Webhooks API

## Folder Structure

VigilGit/

│
├── Backend/
│   ├── main.py           # FastAPI application & GitHub webhook listener
│   ├── scanner.py        # Yelp detect-secrets integration engine
│   └── requirements.txt  # Python package dependencies
│
└── Front-End/
	
    ├── templates/
    │   └── index.html    
    └── static/
        └── logo.svg

## How to Install Application
* **Step 1**: Clone the Github repository and CD:
	git clone https://github.com/Chenna-K/VigilGit.git
	cd VigilGit
* **Step 2**: Navigate to the Backend directory and download dependencies:
	cd Backend
	pip install -r requirements.txt
* **Step 3**: Setup your global environment variables.
* **Step 4**: Run the FastAPI server.	

## License

This project is open-source and avaliable under the MIT License.
