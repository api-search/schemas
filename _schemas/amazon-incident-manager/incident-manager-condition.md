---
description: A conditional statement with which to compare a value, after a timestamp, before a timestamp, or equal to a string or integer. If multiple conditions are specified, the conditionals become an <code>AND</code>ed statement. If multiple values are specified for a conditional, the values are <code>OR</code>d.
layout: schema
name: Condition
properties_list:
- description: ''
  name: after
  type: object
- description: ''
  name: before
  type: object
- description: ''
  name: equals
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-condition-schema.json
slug: incident-manager-condition
source_filename: incident-manager-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-condition-schema.json\",\n  \"title\": \"Condition\",\n  \"description\": \"A conditional statement with which to compare a value, after a timestamp, before a timestamp, or equal to a string or integer. If multiple conditions are specified, the conditionals become an <code>AND</code>ed statement. If multiple values are specified for a conditional, the values are <code>OR</code>d.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"after\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"After the specified timestamp.\"\n        }\n      ]\n    },\n    \"before\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n      \
  \    \"description\": \"Before the specified timestamp\"\n        }\n      ]\n    },\n    \"equals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeValueList\"\n        },\n        {\n          \"description\": \"The value is equal to the provided string or integer. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-condition-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: Condition
---
