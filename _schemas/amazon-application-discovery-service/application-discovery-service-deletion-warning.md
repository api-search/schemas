---
description: DeletionWarning schema from Amazon Application Discovery Service API
layout: schema
name: DeletionWarning
properties_list:
- description: The configuration ID of the configuration item associated with the deletion warning.
  name: configurationId
  type: string
- description: The integer warning code associated with the warning message.
  name: warningCode
  type: integer
- description: A descriptive message of the warning the associated configuration item produced.
  name: warningText
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-deletion-warning-schema.json
slug: application-discovery-service-deletion-warning
source_filename: application-discovery-service-deletion-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-deletion-warning-schema.json\",\n  \"title\": \"DeletionWarning\",\n  \"description\": \"DeletionWarning schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-SERVER-500456\",\n      \"description\": \"The configuration ID of the configuration item associated with the deletion warning.\"\n    },\n    \"warningCode\": {\n      \"type\": \"integer\",\n      \"example\": 1,\n      \"description\": \"The integer warning code associated with the warning message.\"\n    },\n    \"warningText\": {\n      \"type\": \"string\",\n      \"example\": \"Configuration item may have dependencies\",\n      \"description\": \"A descriptive message\
  \ of the warning the associated configuration item produced.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-deletion-warning-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DeletionWarning
---
