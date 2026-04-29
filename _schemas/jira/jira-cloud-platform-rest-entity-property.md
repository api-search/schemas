---
description: An entity property (key-value pair).
layout: schema
name: EntityProperty
properties_list:
- description: The property key.
  name: key
  type: string
- description: The property value (any JSON value).
  name: value
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-entity-property-schema.json
slug: jira-cloud-platform-rest-entity-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityProperty\",\n  \"type\": \"object\",\n  \"description\": \"An entity property (key-value pair).\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The property key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The property value (any JSON value).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-entity-property-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: EntityProperty
---
