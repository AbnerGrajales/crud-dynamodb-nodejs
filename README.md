### NodeJS DynamoDB CRUD
> Project create DYNAMO CRUD with NodeJS

### Configure 

```
Run docker for database DynamoDB
docker-compose up

Create table
dynamodb create-table --cli-input-json file:///{FULL_PATH}/config/tables/table-client.json --endpoint-url http://localhost:8000


cp config/config.sample.js config/config.js 
npm install
npm run start or npm run start:dev

```

### AWS-CLI

```
Get Tables
aws dynamodb list-tables --endpoint-url http://localhost:8000

Create table
dynamodb create-table --cli-input-json file:///{FULL_PATH}/config/tables/table-client.json --endpoint-url http://localhost:8000

Delete Table
aws dynamodb delete-table --table-name CLIENT --endpoint-url http://localhost:8000

```