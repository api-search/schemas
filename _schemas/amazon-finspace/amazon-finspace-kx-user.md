---
description: Represents a user within a FinSpace kdb environment with associated IAM role.
layout: schema
name: KxUser
properties_list:
- description: ''
  name: userArn
  type: string
- description: ''
  name: userName
  type: string
- description: ''
  name: iamRole
  type: string
- description: ''
  name: createTimestamp
  type: string
- description: ''
  name: updateTimestamp
  type: string
- description: ''
  name: environmentId
  type: string
provider_name: Amazon FinSpace
provider_slug: amazon-finspace
schema_file: json-schema/amazon-finspace-kx-user-schema.json
slug: amazon-finspace-kx-user
source_filename: amazon-finspace-kx-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-user-schema.json\",\n  \"title\": \"KxUser\",\n  \"description\": \"Represents a user within a FinSpace kdb environment with associated IAM role.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userArn\": {\n      \"type\": \"string\"\n    },\n    \"userName\": {\n      \"type\": \"string\"\n    },\n    \"iamRole\": {\n      \"type\": \"string\"\n    },\n    \"createTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updateTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"environmentId\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"userName\",\n    \"iamRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-user-schema.json
tags:
- AWS
- Capital Markets
- Data Analytics
- Data Management
- Financial Services
title: KxUser
---
