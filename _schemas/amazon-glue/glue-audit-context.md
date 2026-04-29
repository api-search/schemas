---
description: A structure containing the Lake Formation audit context.
layout: schema
name: AuditContext
properties_list:
- description: ''
  name: AdditionalAuditContext
  type: object
- description: ''
  name: RequestedColumns
  type: object
- description: ''
  name: AllColumnsRequested
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-audit-context-schema.json
slug: glue-audit-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-audit-context-schema.json\",\n  \"title\": \"AuditContext\",\n  \"description\": \"A structure containing the Lake Formation audit context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdditionalAuditContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditContextString\"\n        },\n        {\n          \"description\": \"A string containing the additional audit context information.\"\n        }\n      ]\n    },\n    \"RequestedColumns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditColumnNamesList\"\n        },\n        {\n          \"description\": \"The requested columns for audit.\"\n        }\n      ]\n    },\n    \"AllColumnsRequested\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\
  \n        },\n        {\n          \"description\": \"All columns request for audit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-audit-context-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: AuditContext
---
