---
description: API_Entities_Ci_Variable model
layout: schema
name: API_Entities_Ci_Variable
properties_list:
- description: ''
  name: variable_type
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: protected
  type: boolean
- description: ''
  name: masked
  type: boolean
- description: ''
  name: raw
  type: boolean
- description: ''
  name: environment_scope
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-openapi-original-api_entities_ci_variable-schema.json
slug: gitlab-openapi-original-api_entities_ci_variable
source_filename: gitlab-openapi-original-api_entities_ci_variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_ci_variable-schema.json\",\n  \"title\": \"API_Entities_Ci_Variable\",\n  \"description\": \"API_Entities_Ci_Variable model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"variable_type\": {\n      \"type\": \"string\",\n      \"example\": \"env_var\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"TEST_VARIABLE_1\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"TEST_1\"\n    },\n    \"protected\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"masked\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"raw\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"environment_scope\": {\n      \"type\": \"string\",\n      \"example\": \"*\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_ci_variable-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Ci_Variable
---
