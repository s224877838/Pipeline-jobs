This repository presents a pipeline is designed to automate the software development lifecycle by incorporating stages such as building, testing, code analysis, security scanning, and deployment. The pipeline is triggered using scheduled SCM polling to detect new commits in a time of 1 minute.

Pipeline Trigger

The Jenkins job is configured to poll the GitHub repository at regular intervals. When a new commit is detected, the pipeline is triggered automatically. The commit ID and message are displayed in the console output.

## Pipeline Stages and Tools

The pipeline consists of 7 stages, ewhich are discussed below:
Stage 1: Build
Task is to compile and package the source code.
Tool used is Maven
Stage 2: Unit and Integration Tests
Task is to run unit tests to validate individual components and integration tests to verify component interactions.
Tools used are JUnit (unit testing), Postman (integration testing)
Stage 3 is Code Analysis
Task is to analyze the code for quality, maintainability, and standards compliance.
Tool used is SonarQube
Stage 4 is the Security Scan
Task is to scan the codebase for vulnerabilities and insecure dependencies.
Tool used is OWASP Dependency-Check
Stage 5 is Deploy to Staging
Task is to deploy the application to a staging environment.
Tool used is AWS CLI
Stage 6 is Integration Tests on Staging
Task is to execute integration tests in a staging environment to ensure production readiness.
Tool used is Selenium
Stage 7 is to deploy to Production
Task is to deploy the final application build to the production environment.
Tool used is AWS CLI

