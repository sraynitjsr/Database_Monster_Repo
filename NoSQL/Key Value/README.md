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
