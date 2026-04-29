---
description: Use the AttributeValueList to filter by string or integer values.
layout: schema
name: AttributeValueList
properties_list:
- description: ''
  name: integerValues
  type: object
- description: ''
  name: stringValues
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-attribute-value-list-schema.json
slug: incident-manager-attribute-value-list
source_filename: incident-manager-attribute-value-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-attribute-value-list-schema.json\",\n  \"title\": \"AttributeValueList\",\n  \"description\": \"Use the AttributeValueList to filter by string or integer values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"integerValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerList\"\n        },\n        {\n          \"description\": \"The list of integer values that the filter matches.\"\n        }\n      ]\n    },\n    \"stringValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The list of string values that the filter matches.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-attribute-value-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: AttributeValueList
---
