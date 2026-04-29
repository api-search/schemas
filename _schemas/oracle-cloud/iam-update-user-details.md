---
description: UpdateUserDetails schema from oracle-cloud-iam-openapi.yaml
layout: schema
name: UpdateUserDetails
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: email
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/iam-update-user-details-schema.json
slug: iam-update-user-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-update-user-details-schema.json\",\n  \"title\": \"UpdateUserDetails\",\n  \"description\": \"UpdateUserDetails schema from oracle-cloud-iam-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"admin@example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-update-user-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: UpdateUserDetails
---
