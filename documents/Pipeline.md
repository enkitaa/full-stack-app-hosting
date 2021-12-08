## Application Pipeline

![Pipeline_architecture](..\screenshots\Pipeline_arch.png)

### CI/CD

#### GitHub
Github repository of the application is linked to the CircleCI account.
On code push by a developer in the main branch CI/CD pipeline is trigerred automatically to deploy the application. The same can be done manually also.

#### CircleCI
CircleCI is configured using `.circleci/config.yml` which controls the flow of the pipeline. 

- **Orbs**: Defined to install the dependencies such as node and aws cli.
- **Jobs**: Following processes are done through defined jobs,
1) Node install, asw cli setup, eb cli 
2) Frontend - package installation, application build, application deploy to S3 bucket.
3) Backend - package installation, application build, application build zip deploy to Elastic beanstalk.