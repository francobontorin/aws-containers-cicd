# Amazon CI/CD Pipeline
Directions on how to launch this sample app on Amazon ECS can be found in the documentation: [Docker basics](http://docs.aws.amazon.com/AmazonECS/latest/developerguide/docker-basics.html).

# Introduction
Fork from https://github.com/awslabs/ecs-refarch-continuous-deployment that adds new components such as GhostInspector used fro Automated UI testing, a Lex chatbot integrated with a slack channel that manages and trigger deployments.

# Objectives
* Create an automated CI/CD Pipeline where every commit will trigger a set of actions that builds a container image, test, validate and promote the build image to different stages
* Use rolling updates mechanisms and blue/green deployments to enable application updates with zero downtime
* Demonstrate how DevOps can be achieved within AWS and how serverless can be used to automate the deployment and self heal the application in case of a non standard change
* Integrate a Chatbot on Slack as an orchestrator that can trigger deployments and gather the status of the pipeline
* Have all the services and artifacts as code via CloudFormation enabling the whole infrastructure to be recreated in a matter of minutes

# CICD Architecture

![Alt text](http://prod.octankcorp.com/_images/cicd_architecture.png "CI/CD Architecture")

# Auto Healing/Blue Green

![Alt text](http://prod.octankcorp.com/_images/ah_architecture.png "Blue/Green Architecture")

# Lex Architecture

![Alt text](http://prod.octankcorp.com/_images/lex.png "Lex Architecture")

# Author

Franco Bontorin - 
Solutions Architect

# License

This is under GNU GPL v2

# Date

April 2017
