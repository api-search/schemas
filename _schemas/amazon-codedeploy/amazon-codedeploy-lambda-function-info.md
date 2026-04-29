---
description: Information about a Lambda function specified in a deployment.
layout: schema
name: LambdaFunctionInfo
properties_list:
- description: ''
  name: functionName
  type: object
- description: ''
  name: functionAlias
  type: object
- description: ''
  name: currentVersion
  type: object
- description: ''
  name: targetVersion
  type: object
- description: ''
  name: targetVersionWeight
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-lambda-function-info-schema.json
slug: amazon-codedeploy-lambda-function-info
source_filename: amazon-codedeploy-lambda-function-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-lambda-function-info-schema.json\",\n  \"title\": \"LambdaFunctionInfo\",\n  \"description\": \" Information about a Lambda function specified in a deployment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionName\"\n        },\n        {\n          \"description\": \" The name of a Lambda function. \"\n        }\n      ]\n    },\n    \"functionAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionAlias\"\n        },\n        {\n          \"description\": \" The alias of a Lambda function. For more information, see <a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/aliases-intro.html\\\">Lambda Function Aliases</a> in\
  \ the <i>Lambda Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"currentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \" The version of a Lambda function that production traffic points to. \"\n        }\n      ]\n    },\n    \"targetVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \" The version of a Lambda function that production traffic points to after the Lambda function is deployed. \"\n        }\n      ]\n    },\n    \"targetVersionWeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficWeight\"\n        },\n        {\n          \"description\": \" The percentage of production traffic that the target version of a Lambda function receives. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-lambda-function-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: LambdaFunctionInfo
---
