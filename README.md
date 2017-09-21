# lambda-wkhtmltopdf
Convert HTML to PDF using wkhtmltopdf on AWS Lambda

## Input

```json
{
    "data" : "<h1>Claudemiro</h1>",
    "filename": "optional filename",
    "pagesize": "optional pagesize default: a4",
    "bucket": "s3 bucket to use for output"
}
```

## Output

```json
{
    "filename": "8rqj9td0pvjf9a4i.pdf"
}
```

## Configuration

1. Make sure AWS Lambda function has `PutObject` access to S3 bucket
2. Download the binary wkhtmltopdf for linux-x64 and put in the current directory
3. Run npm install
4. Zip everything and upload to aws-lambda

## Links

* http://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-mapping-template-reference.html
* http://aws.amazon.com/documentation/apigateway/
* http://wkhtmltopdf.org/
* https://www.npmjs.com/package/wkhtmltopdf
* http://swagger.io/
* https://github.com/ashiina/lambda-local
