# My Widget Service
## Creating a serverless application using the AWS CDK
Simple widget dispensing service. Includes:
* An AWS Lambda function.
* An Amazon API Gateway API to call the Lambda function.
* An Amazon S3 bucket that holds the widgets.

### Config
* Add config values to `.config`:

    `export AWS_USER=`

    `export AWS_REGION=`

    `export AWS_ACCESS_KEY_ID=`

    `export AWS_SECRET_ACCESS_KEY=`

* Run `./aws_configure.sh`

### Bootstrap
* Run `./aws_bootstrap.sh`

### Deploy
* Run `./deploy.sh`

* If the deployment succeeds, an URL appears in one of the last lines in the window. Use this URL to run the service.

### Run
curl -X GET '$URL'

curl -X POST '$URL/example'

curl -X GET '$URL'

curl -X GET '$URL/example'

curl -X DELETE '$URL/example'

curl -X GET '$URL'


source: https://docs.aws.amazon.com/cdk/v2/guide/serverless_example.html