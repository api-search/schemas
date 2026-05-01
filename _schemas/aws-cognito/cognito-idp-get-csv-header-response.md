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
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-csv-header-response-schema.json
slug: cognito-idp-get-csv-header-response
source_filename: cognito-idp-get-csv-header-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool that the users are to be imported into.\"\n        }\n      ]\n    },\n    \"CSVHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfStringTypes\"\n        },\n        {\n          \"description\": \"The header information of the CSV file for the user import job.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response from the server to the request to get the header information of the CSV file for the user import job.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-csv-header-response-schema.json\",\n  \"title\": \"GetCSVHeaderResponse\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-csv-header-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetCSVHeaderResponse
---
