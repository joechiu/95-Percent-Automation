# 95-Percent-Automation 
## 95% Automation
This commitment is a sample to create a demo task which is able to finish the assigned job by 95% automation process including automation infrastructure, application installations, deployment, CI / CD solutions, tests and version control.

## Summary
- update the your-task by your task in each of the codes, yml files and configurations.
- this task is built for the Job TechChallengeApp.
- the automation tasks include automation infrastructure, application installations, deployment, CI / CD solutions, tests and version control.
- the automation processes for this sample are tested and running.
- the app run by golang, however it's partially working and provides limited functions in my experiment.
- the infrastructure codes for creating VM and connection to GCP.
- a TechChallengeApp application running on port 3000.
- docker postgrs db running on port 5432
- docker Jenkins running on port 8080
- a testing Jenkins site is available for showing CI / CD test.
- Ansible playbook used as IaC for the automation.

## Pre-Requisite
- GCP account for IaC
- Ansible service environment
- Github for Jenkins integration
- gcloud enabled (optional)

## RUN
- git clone https://github.com/joechiu/95-Percent-Automation
- cd auto-infrastructure
- ansible-playbook -i hosts playbook.yml
- it will create an instance called demo in your GCP compute engine
- get the IP address in the demo instance
- Jenkins: http://xxx.xxx.xxx.xxx:8080/ (replace the xxx with the IP address)
- login with admin/foobar
- build JobDemo to see the CI / CD process

## Showcase
- This showcase will be presenting to the customers about how will be the application integration and deployment done by Jenkins CI / CD and raising the version tag to push to the forked repository if the case succeeds.
- The stages for this case include "Start Task", "Update Change", "Preload for Deployment", "Init Working Env", "Deploy Application", "Preload for Testing", "Skipping Create", "Testing Read", "Skipping Update", "Testing Delete" and "Commit Version Change".
- Any commitments submitted to the forked repository the Jenkins pipeline will trigger the deployment process to install the application.
![Installed case sample](https://github.com/joechiu/95-Percent-Automation/blob/main/images/app-dump.PNG?raw=true)
- Right after deployed the application, it will start to testing the API which can include unit test, load testing performance test and integration test, for example. 
![An example for this showcase](https://github.com/joechiu/95-Percent-Automation/blob/main/images/jenkins-demo-app-dump.PNG?raw=true)
- Once complete the test, the root.go code version will be increased by 1 and pushed into the forked repository to complete the showcase.
![The stages for this case](https://github.com/joechiu/95-Percent-Automation/blob/main/images/jenkins-demo.PNG?raw=true)

## TODO
- fix the bugs if exist.
- use an elegant domain name.
- 100% automation.

## Links
- task documentation github:  https://github.com/joechiu/95-Percent-Automation
- forked application github: https://github.com/joechiu/95-Percent-Automation
- Jenkins demo site: http://xxx.xxx.xxx.xxx:8080/ (replace the xxx with the IP address)
- application URL: http://xxx.xxx.xxx.xxx:3000/(replace the xxx with the IP address) 
