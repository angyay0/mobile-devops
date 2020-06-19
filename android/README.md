# Welcome
This file contains examples to create CI/CD experiences for Android target.

The first task is upload our android repository if we want to keep track inside Azure DevOps, but we can use other sources instead.

### Continuous Integration
The first thing is connecting the repo, we can choose from different sources.
!["Repo Connection"](img/00.png "Repo Connection")

The prebuilt template for android contains all the required steps to generate a non-signed apk.
!["Task Template"](img/01.png "Task Template")

For generate a signed apk, we must provision the jks file and credentials for signing the build
!["Signing Configuration"](img/02.png "Signing Configuration")

The agent for running the pipeline, it will run in almost every agent, but for best result choose mac or linux distribution
!["Agent Selection"](img/03.png "Agent Selection")


Last step is save and queue pipeline

!["Save Pipeline"](img/04.png "Save Pipeline")

Build Results
!["Results"](img/05.png "Results")



### Continuous Delivery
Currently exist some steps, but for integrating with Official Stores we highly recommend working with AppCenter CD.
