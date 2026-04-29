---
description: List of access credentials.
layout: schema
name: CredentialList
properties_list:
- description: Array of credentials.
  name: credentials
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/business-api-credential-list-schema.json
slug: business-api-credential-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-credential-list-schema.json\",\n  \"title\": \"CredentialList\",\n  \"description\": \"List of access credentials.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"credentials\": {\n      \"type\": \"array\",\n      \"description\": \"Array of credentials.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An access control credential.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the credential.\",\n            \"example\": \"cred-001\"\n          },\n          \"userId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the user this credential belongs to.\",\n            \"example\": \"usr-001\"\n          },\n          \"type\": {\n          \
  \  \"type\": \"string\",\n            \"description\": \"Type of credential.\",\n            \"enum\": [\n              \"badge\",\n              \"pin\",\n              \"biometric\",\n              \"mobile\"\n            ],\n            \"example\": \"badge\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Credential status.\",\n            \"enum\": [\n              \"active\",\n              \"suspended\",\n              \"expired\"\n            ],\n            \"example\": \"active\"\n          },\n          \"validFrom\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Start of credential validity period.\"\n          },\n          \"validTo\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"End of credential validity period.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-credential-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: CredentialList
---
