---
description: Request body for updating a global target property.
layout: schema
name: GlobalTargetPropertyUpdateRequest
properties_list:
- description: ''
  name: propertyDisplayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: validValues
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-global-target-property-update-request-schema.json
slug: oracle-enterprise-manager-cloud-control-global-target-property-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GlobalTargetPropertyUpdateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a global target property.\",\n  \"properties\": {\n    \"propertyDisplayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"validValues\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-global-target-property-update-request-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: GlobalTargetPropertyUpdateRequest
---
