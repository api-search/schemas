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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-user-import-jobs-response-schema.json
slug: user-pools-list-user-import-jobs-response
source_filename: user-pools-list-user-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-user-import-jobs-response-schema.json\",\n  \"title\": \"ListUserImportJobsResponse\",\n  \"description\": \"Represents the response from the server to the request to list the user import jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserImportJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobsListType\"\n        },\n        {\n          \"description\": \"The user import jobs.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"An identifier that can be used to return the next set of user import jobs in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-user-import-jobs-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ListUserImportJobsResponse
---
