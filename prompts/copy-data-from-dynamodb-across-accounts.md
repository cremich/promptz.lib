# Copy data from DynamoDB across accounts

Create a shell script to copy all data from a source DynamoDB table into a target DynamoDB table using the AWS CLI. Source and target tables are provisioned in different AWS accounts. 

- Use named profiles called "source" and "target" to connect to the target and source account.
- Save scan results to a temporary directory
- Processing each item individually
