---
description: Represents the response from the server to the request to start the user import job.
layout: schema
name: StartUserImportJobResponse
properties_list:
- description: ''
  name: UserImportJob
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-start-user-import-job-response-schema.json
slug: user-pools-start-user-import-job-response
source_filename: user-pools-start-user-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-start-user-import-job-response-schema.json\",\n  \"title\": \"StartUserImportJobResponse\",\n  \"description\": \"Represents the response from the server to the request to start the user import job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserImportJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobType\"\n        },\n        {\n          \"description\": \"The job object that represents the user import job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-start-user-import-job-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: StartUserImportJobResponse
---
