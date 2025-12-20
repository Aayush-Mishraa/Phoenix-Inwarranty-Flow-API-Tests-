
# Postman API Automation Integration with GitHub Actions

This restrates a Proof of Concept (POC) for integrating Postman API automation tests with GitHub Actions.

The API tests are written in Postman and executed using Newman along with the newman-reporter-htmlextra. GitHub Actions automates the execution on every push to the main branch, via manual trigger using workflow_dispatch, and through scheduled runs using cron jobs.

---

## CI/CD Execution and Reporting

* Postman collections are executed using Newman
* HTML execution reports are generated using newman-reporter-htmlextra
* Test reports are archived as GitHub Artifacts for download
* Reports are published using GitHub Pages for easy access
* Email notifications are sent to team members using Gmail SMTP
* GitHub Actions manages the complete automation workflow

---

## Deployment and Reports

All deployments:
[https://github.com/Aayush-Mishraa/Phoenix-Inwarranty-Flow-API-Tests-/deployments](https://github.com/Aayush-Mishraa/Phoenix-Inwarranty-Flow-API-Tests-/deployments)

Latest HTML report (GitHub Pages):
[https://aayush-mishraa.github.io/Phoenix-Inwarranty-Flow-API-Tests-/](https://aayush-mishraa.github.io/Phoenix-Inwarranty-Flow-API-Tests-/)

![Postman Report](https://raw.githubusercontent.com/Aayush-Mishraa/Phoenix-Inwarranty-Flow-API-Tests-/static-content/Report.png)


---

## About Me

My name is Aayush Mishra, and I have 5 years of experience in QA Automation and API testing with CI/CD integration.

My skill set includes:

* UI Automation using Selenium WebDriver, Cypress, and Playwright
* API Automation using Postman and Newman
* CI/CD automation using GitHub Actions
* Test reporting and email notifications
* Secrets management using GitHub Secrets

Connect with me:
LinkedIn: [https://www.linkedin.com/in/aayushmishra33/](https://www.linkedin.com/in/aayushmishra33/)
Website: [https://aayushmishra.tech/home](https://aayushmishra.tech/home)

---

## Testing Coverage

* Happy flow testing
* Negative and edge case testing
* Authentication and token testing
* Data-driven testing using CSV
* Schema validation
* Secure secrets management

---

## Technology Stack

* Postman
* Node.js (v22)
* Newman
* Newman Reporter HTML Extra
* GitHub Actions
* Gmail SMTP
* GitHub Pages
* CSV-based data-driven testing
* AWS EC2 self-hosted GitHub runner

---

## HTML Report

The HTML report is generated inside the newman folder after execution.
The latest report is always available via GitHub Pages, while previous reports can be downloaded from GitHub Artifacts.

---

## Project Structure

```
Phoenix Inwarranty Flow
├── Inwarranty-flow Collection.postman_collection.json
├── QA.postman_environment.json
└── testdata.csv
```

---

## How to Run the Project Locally

Clone the repository:

```
git clone https://github.com/Aayush-Mishraa/Phoenix-Inwarranty-Flow-API-Tests-.git
```

Install Node.js and npm from:
[https://nodejs.org/en](https://nodejs.org/en)

Install Newman:

```
npm install -g newman
```

Install Newman Reporter HTML Extra:

```
npm install -g newman-reporter-htmlextra
```

Run the Newman command:

```
newman run "Inwarranty-flow Collection.postman_collection.json" \
  -e QA.postman_environment.json \
  -d testdata.csv \
  -r cli,htmlextra \
  --reporter-htmlextra-export ./newman/index.html
```


> *If there is anything I can improve, I am always open to feedback and continuously eager to learn and innovate with new technologies. Thank you.*
>
> **Connect with me:**
> LinkedIn: [https://www.linkedin.com/in/aayushmishra33/](https://www.linkedin.com/in/aayushmishra33/)
>
> Website: [https://aayushmishra.tech/home](https://aayushmishra.tech/home)
>
> Email: [aayushmishra026@gmail.com](mailto:aayushmishra026@gmail.com)




