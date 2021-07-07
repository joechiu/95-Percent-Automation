# 95-Percent-Automation 
## 95% Automation
This commitment is a sample aims to accomplish a demo tasks by 95% automation CI / CD process. The tasks includes automation infrastructure, application installations, VM deployment, CI / CD solutions, tests and version control.

## Summary
- update the changes in the your-task directory to meet your requirements in each of the codes, yml files and configurations.
- this task is built for the Job TechChallengeApp for a demonstration purpose.
- the automation tasks include automation infrastructure, application installations, deployment, CI / CD solutions, tests and version control.
- the automation processes for this sample are tested and running.
- the app is run by golang, however it's partially working and provides limited functions as my experiment.
- the infrastructure codes for creating VM and connection to GCP.
- a TechChallengeApp application running on port 3000.
- docker postgres db running on port 5432
- docker Jenkins running on port 8080
- a testing Jenkins site is available for showing CI / CD tests.
- Ansible playbooks run as IaC for the CI / CD automation.

## Pre-Requisite
- Jenkins
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
- This showcase will be presenting to the customers about how the application integration and deployment are done by Jenkins CI / CD and updating a version tag then pushing to the github repository if the case succeeds.
- The stages for this case include "Start Task", "Update Change", "Preload for Deployment", "Init Working Env", "Deploy Application", "Preload for Testing", "Skipping Create", "Testing Read", "Skipping Update", "Testing Delete" and "Commit Version Change".
- Any commitments submitted to the github repository, the Jenkins pipeline will trigger the deployment process to install the application.
- Right after deployed the application, it will start testing the API which can include unit tests, load testing performance tests and integration tests, for example. 
- Once the test completed, the root.go code version will be increased by 1 and pushed into the forked repository to complete the user case.

## TODO
- fix bugs if exist.
- use an elegant domain name.
- 100% automation.

## Links
- task documentation github:  https://github.com/joechiu/95-Percent-Automation
- forked application github: https://github.com/joechiu/95-Percent-Automation
- Jenkins demo site: http://xxx.xxx.xxx.xxx:8080/ (replace the xxx with your IP address)
- application URL: http://xxx.xxx.xxx.xxx:3000/(replace the xxx with your IP address) 

## Contributors

You are free to update these tools to make this project more useful and helpful.

## License

A short snippet describing the license (MIT, Apache, etc.)
