---
description: Represents the request to list the user import jobs.
layout: schema
name: ListUserImportJobsRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: PaginationToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-user-import-jobs-request-schema.json
slug: user-pools-list-user-import-jobs-request
source_filename: user-pools-list-user-import-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-user-import-jobs-request-schema.json\",\n  \"title\": \"ListUserImportJobsRequest\",\n  \"description\": \"Represents the request to list the user import jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool that the users are being imported into.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolQueryLimitType\"\n        },\n        {\n          \"description\": \"The maximum number of import jobs you want the request to return.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to <code>ListUserImportJobs</code>, which can be used to return the next set of import jobs in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"MaxResults\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-user-import-jobs-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListUserImportJobsRequest
---
