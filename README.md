# beyonnex-qa
This repository is providing solution of beyonnex challenge. This repository Automation Test cases with docker file using Cypress.

**Automation Test Scripts:**

That contains automated test scripts for testing of GUI automation for a web application using Docker Node.js and npm.

**Tools and Technologies**

Language: JavaScript
Automation Framework: NPM Node JS
Reporting: Mochawesome

**Framework Approach**

The test automation framework follows a node structure to enhance code reusability, maintainability, and readability. It's designed to organize the test scripts effectively.

**Folder Struture & Test Cases:**

**e2e:** Folder contains weathershooper.cy.js contains implementation of weather shooper test

**Videos:** Folder contains all the execution video of steps.

**package.json and package-lock.json**: Node.js package configuration files. They include dependencies and scripts for running Cypress tests.

**report** : This folder contains mochawesome report 

**Setup and Execution Steps**

1) git clone https://github.com/Razacs/beyonnex-qa.git

2) cd weathershopper  

3) npm install // to install all dependencies

(npm install --save-dev mocha mochawesome mochawesome-merge mochawesome-report-generator) //Install Dependecies

4) npm run cypress:run // Execute all test cases

5) npm run test (to Execute agd get moachaswesome report) 
   
**To Execute with Docker**

1) **Build the Docker Image**

docker build -t weathershopper .

2) **Run the Docker Container**

docker run -it --rm -v ${PWD}:/app -v /dev/shm:/dev/shm weathershopper

3) docker logs [container_id] //Replace container id with actual ID

----> To find container ID execute this command (**docker ps -a**)

4) In case of keep containers from being automatically removed, I remove the --rm option from docker run command, then after execution container will not removed.

docker run -it -v ${PWD}:/app -v /dev/shm:/dev/shm weathershopper

**Output:**

![image](https://github.com/Razacs/beyonnex-qa/assets/32739941/e2e4d989-110e-4ec2-9bea-c47bc5d33a03)

![image](https://github.com/Razacs/beyonnex-qa/assets/32739941/fadc5c66-1b35-4a13-aec4-dc7576b86d91)

![image](https://github.com/Razacs/beyonnex-qa/assets/32739941/46b85cc4-9fd6-4466-abcf-2a7c29d8dae0)

![image](https://github.com/Razacs/beyonnex-qa/assets/32739941/7b6c265e-1525-430c-8fdc-02b8849ab6d3)

![image](https://github.com/Razacs/beyonnex-qa/assets/32739941/d8ff25f7-879b-4006-91e5-b43c8da733fe)

![image](https://github.com/Razacs/beyonnex-qa/assets/32739941/c1f63fb8-8711-4c06-a498-e89363d2a849)

**Let me know if you need any further information from my side.

Thanks!**
