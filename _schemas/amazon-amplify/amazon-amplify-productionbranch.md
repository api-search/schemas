---
description: ''
layout: schema
name: ProductionBranch
properties_list:
- description: ''
  name: branchName
  type: string
- description: ''
  name: lastDeployTime
  type: string
- description: ''
  name: status
  type: string
provider_name: Amazon Amplify
provider_slug: amazon-amplify
schema_file: json-schema/amazon-amplify-productionbranch-schema.json
slug: amazon-amplify-productionbranch
source_filename: amazon-amplify-productionbranch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ProductionBranch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchName\": {\n      \"type\": \"string\"\n    },\n    \"lastDeployTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/json-schema/amazon-amplify-productionbranch-schema.json
tags:
- Frontend
- Full Stack
- Hosting
- Mobile Development
- Web Applications
title: ProductionBranch
---
