---
description: Represents the request to describe the user import job.
layout: schema
name: DescribeUserImportJobRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: JobId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-describe-user-import-job-request-schema.json
slug: user-pools-describe-user-import-job-request
source_filename: user-pools-describe-user-import-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-import-job-request-schema.json\",\n  \"title\": \"DescribeUserImportJobRequest\",\n  \"description\": \"Represents the request to describe the user import job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool that the users are being imported into.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobIdType\"\n        },\n        {\n          \"description\": \"The job ID for the user import job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-describe-user-import-job-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DescribeUserImportJobRequest
---
