---
description: Request body for creating a global target property.
layout: schema
name: GlobalTargetPropertyCreateRequest
properties_list:
- description: ''
  name: propertyName
  type: string
- description: ''
  name: propertyDisplayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: propertyType
  type: string
- description: ''
  name: validValues
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-global-target-property-create-request-schema.json
slug: oracle-enterprise-manager-cloud-control-global-target-property-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GlobalTargetPropertyCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a global target property.\",\n  \"properties\": {\n    \"propertyName\": {\n      \"type\": \"string\"\n    },\n    \"propertyDisplayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"propertyType\": {\n      \"type\": \"string\"\n    },\n    \"validValues\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-global-target-property-create-request-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: GlobalTargetPropertyCreateRequest
---
