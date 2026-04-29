---
description: API_Entities_ApplicationWithSecret model
layout: schema
name: API_Entities_ApplicationWithSecret
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: application_id
  type: string
- description: ''
  name: application_name
  type: string
- description: ''
  name: callback_url
  type: string
- description: ''
  name: confidential
  type: boolean
- description: ''
  name: secret
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-applications-api_entities_application-with-secret-schema.json
slug: gitlab-api-v4-applications-api_entities_application-with-secret
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-applications-api_entities_application-with-secret-schema.json\",\n  \"title\": \"API_Entities_ApplicationWithSecret\",\n  \"description\": \"API_Entities_ApplicationWithSecret model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"123456\"\n    },\n    \"application_id\": {\n      \"type\": \"string\",\n      \"example\": \"5832fc6e14300a0d962240a8144466eef4ee93ef0d218477e55f11cf12fc3737\"\n    },\n    \"application_name\": {\n      \"type\": \"string\",\n      \"example\": \"MyApplication\"\n    },\n    \"callback_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://redirect.uri\"\n    },\n    \"confidential\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"secret\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"ee1dd64b6adc89cf7e2c23099301ccc2c61b441064e9324d963c46902a85ec34\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-applications-api_entities_application-with-secret-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_ApplicationWithSecret
---
