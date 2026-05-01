---
description: Represents the response from the server to the request to create the user import job.
layout: schema
name: CreateUserImportJobResponse
properties_list:
- description: ''
  name: UserImportJob
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-create-user-import-job-response-schema.json
slug: cognito-idp-create-user-import-job-response
source_filename: cognito-idp-create-user-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserImportJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobType\"\n        },\n        {\n          \"description\": \"The job object that represents the user import job.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response from the server to the request to create the user import job.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-import-job-response-schema.json\",\n  \"title\": \"CreateUserImportJobResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-user-import-job-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateUserImportJobResponse
---
