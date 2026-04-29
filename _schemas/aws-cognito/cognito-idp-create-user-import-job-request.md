---
description: Represents the request to create the user import job.
layout: schema
name: CreateUserImportJobRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: CloudWatchLogsRoleArn
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-create-user-import-job-request-schema.json
slug: cognito-idp-create-user-import-job-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobNameType\"\n        },\n        {\n          \"description\": \"The job name for the user import job.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool that the users are being imported into.\"\n        }\n      ]\n    },\n    \"CloudWatchLogsRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The role ARN for the Amazon CloudWatch Logs Logging role for the user import job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\",\n    \"UserPoolId\",\n    \"CloudWatchLogsRoleArn\"\n  ],\n  \"description\": \"Represents the request\
  \ to create the user import job.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-import-job-request-schema.json\",\n  \"title\": \"CreateUserImportJobRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-import-job-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateUserImportJobRequest
---
