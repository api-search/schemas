---
description: Configuration for failed invocation destinations. Specify an SQS queue or SNS topic to receive records of failed asynchronous invocations or event source mapping batches.
layout: schema
name: DestinationConfig
properties_list:
- description: ''
  name: OnSuccess
  type: object
- description: ''
  name: OnFailure
  type: object
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-destination-config-schema.json
slug: aws-lambda-destination-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DestinationConfig\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for failed invocation destinations. Specify an SQS queue or SNS topic to receive records of failed asynchronous invocations or event source mapping batches.\",\n  \"properties\": {\n    \"OnSuccess\": {\n      \"type\": \"object\"\n    },\n    \"OnFailure\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-destination-config-schema.json
tags: []
title: DestinationConfig
---
