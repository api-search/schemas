---
description: A stored credential for workflow execution
layout: schema
name: Credential
properties_list:
- description: Unique credential identifier
  name: id
  type: string
- description: Windows login username
  name: username
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-credential-schema.json
slug: alteryx-server-v3-credential
source_filename: alteryx-server-v3-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Credential\",\n  \"type\": \"object\",\n  \"description\": \"A stored credential for workflow execution\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique credential identifier\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Windows login username\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-credential-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: Credential
---
