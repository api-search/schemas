---
description: Represents the response from the server to the request to get the header information of the CSV file for the user import job.
layout: schema
name: GetCSVHeaderResponse
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: CSVHeader
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-csv-header-response-schema.json
slug: user-pools-get-csv-header-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-csv-header-response-schema.json\",\n  \"title\": \"GetCSVHeaderResponse\",\n  \"description\": \"Represents the response from the server to the request to get the header information of the CSV file for the user import job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool that the users are to be imported into.\"\n        }\n      ]\n    },\n    \"CSVHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfStringTypes\"\n        },\n        {\n          \"description\": \"The header information of the CSV file for the user import job.\"\n        }\n     \
  \ ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-csv-header-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetCSVHeaderResponse
---
