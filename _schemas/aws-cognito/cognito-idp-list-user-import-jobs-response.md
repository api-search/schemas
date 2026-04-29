---
description: Represents the response from the server to the request to list the user import jobs.
layout: schema
name: ListUserImportJobsResponse
properties_list:
- description: ''
  name: UserImportJobs
  type: object
- description: ''
  name: PaginationToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-user-import-jobs-response-schema.json
slug: cognito-idp-list-user-import-jobs-response
source_filename: cognito-idp-list-user-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserImportJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobsListType\"\n        },\n        {\n          \"description\": \"The user import jobs.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"An identifier that can be used to return the next set of user import jobs in the list.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response from the server to the request to list the user import jobs.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-import-jobs-response-schema.json\",\n  \"title\": \"ListUserImportJobsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-import-jobs-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListUserImportJobsResponse
---
