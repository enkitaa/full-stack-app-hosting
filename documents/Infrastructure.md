## Application Infrastructure

### Deploment Platform - AWS

![Infrastructure_architecture](screenshots\Infra_arch.png)

#### RDS Postgres

AWS RDS with PostgresEngine is set up as database for the application to store and retrieve data.

Database endpoint: `udagram.cbciv312qkyq.us-east-1.rds.amazonaws.com` Port: `5432`

#### Elastic Beanstalk

AWS Elastic Beanstack is setup for deployment of backend Nodejs application. The application build is uploaded as an archived file to EB. 

EB URL: `http://ugapi.us-east-1.elasticbeanstalk.com/`

#### S3 Bucket

AWS S3 Bucket is used to host the frontend application using its static web hosting capabilities.

Another S3 bucket is configured to host the uploaded pictures from client in the application.

Users can access the application from the Bucket URL.

Application URL(S3 bucket): `http://udagram-frontend1.s3-website-us-east-1.amazonaws.com`

