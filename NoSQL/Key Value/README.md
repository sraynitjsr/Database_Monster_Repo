# Dynamo DB is a Key Value Based NoSQL DB

# First DynamoDB Query
{
    "TableName": "Movies",
    "KeyConditionExpression": "#yr = :year",
    "ExpressionAttributeNames": {
        "#yr": "Year"
    },
    "ExpressionAttributeValues": {
        ":year": {
            "N": "2020"
        }
    }
}

## DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services (AWS). It is designed for applications that require seamless and low-latency performance at any scale. Here are some key features and aspects of DynamoDB:

#### NoSQL Database: DynamoDB is a NoSQL database, which means it doesn't rely on traditional relational database models. Instead, it uses a flexible schema and supports semi-structured data.

#### Managed Service: DynamoDB is fully managed by AWS, which means that AWS takes care of tasks like server provisioning, patching, and backups, allowing developers to focus on building their applications.

#### Scalability: DynamoDB is designed to scale horizontally, which means it can automatically handle increased workloads as your application grows. You can adjust your read and write capacity to meet your application's needs.

#### Data Models: DynamoDB supports key-value and document data models. You can create tables with flexible schema designs to fit your application's data storage requirements.

#### Consistency Models: DynamoDB offers two consistency models: eventually consistent reads and strongly consistent reads. Eventually consistent reads provide low-latency access, while strongly consistent reads ensure that you always get the most recent data but might have higher latency.

#### Global Tables: DynamoDB allows you to create global tables that can be replicated across multiple AWS regions. This enables you to provide low-latency access to users in different parts of the world.

#### Security: DynamoDB provides features for data encryption at rest and in transit. You can also use AWS Identity and Access Management (IAM) to control who can access your data.

#### On-Demand and Provisioned Capacity: You can choose between on-demand and provisioned capacity modes. On-demand capacity automatically adjusts to your application's traffic, while provisioned capacity requires you to specify and manage the read and write capacity units.

#### Triggers and Streams: DynamoDB supports triggers and streams, which allow you to respond to changes in the data by triggering AWS Lambda functions or other actions when records are added, updated, or deleted.

#### Pay-as-You-Go: DynamoDB pricing is based on the actual usage of the service, so you only pay for the read and write capacity you consume.

#### DynamoDB is a popular choice for web and mobile applications, gaming, IoT, and any application that requires fast and flexible data storage and retrieval. Its ability to handle large-scale, low-latency workloads and its integration with other AWS services make it a powerful choice for developers building applications in the AWS ecosystem.
