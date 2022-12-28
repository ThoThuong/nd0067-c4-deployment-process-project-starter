## Udagram Infrastructure

![Architecture](architecture.png)

### AWS
#### RDS Postgres
The application server uses AWS RDS Postgres as database for storing and retrieving information.

Database URI: `postgres.cfjjvm1o2xaj.ap-southeast-1.rds.amazonaws.com`

#### Elastic Beanstalk
The application server is deployed on AWS Elastic Beanstalk service. The application is build, archived and uploaded
to and S3 bucket from where Elastic Beanstalk extracts and runs the application on an endpoint.

EB URL: `http://thuong-api-3.eba-gcfruuaa.ap-southeast-1.elasticbeanstalk.com/api/v0`

#### S3 Bucket
The frontend application is deployed using AWS S3 Bucket. The bundled assets are uploaded to an S3 bucket and that
bucket is made publicly readable.

Bucket URL: `http://thuongtn3-udacity-nano.s3-website-ap-southeast-1.amazonaws.com`

End users can access the application from the Bucket URL.