---
description: The result of processing an import set record including the transformation outcome.
layout: schema
name: ImportSetResult
properties_list:
- description: The name of the transform map used to process the record.
  name: transform_map
  type: string
- description: The target table into which the record was transformed.
  name: table
  type: string
- description: The display name of the transform map.
  name: display_name
  type: string
- description: The display value of the target record created or updated.
  name: display_value
  type: string
- description: A link to the target record in ServiceNow.
  name: record_link
  type: string
- description: The transformation status. Common values include inserted, updated, error, and ignored.
  name: status
  type: string
- description: A descriptive message about the transformation result, especially useful when the status is error.
  name: status_message
  type: string
- description: The sys_id of the import set row record in the staging table.
  name: sys_id
  type: string
- description: The sys_id of the record created or updated in the target table.
  name: target_sys_id
  type: string
- description: The sys_id of the parent import set.
  name: import_set
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-import-set-import-set-result-schema.json
slug: servicenow-import-set-import-set-result
source_filename: servicenow-import-set-import-set-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of processing an import set record including the transformation outcome.\",\n  \"properties\": {\n    \"transform_map\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the transform map used to process the record.\",\n      \"example\": \"example_value\"\n    },\n    \"table\": {\n      \"type\": \"string\",\n      \"description\": \"The target table into which the record was transformed.\",\n      \"example\": \"example_value\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the transform map.\",\n      \"example\": \"example_value\"\n    },\n    \"display_value\": {\n      \"type\": \"string\",\n      \"description\": \"The display value of the target record created or updated.\",\n      \"example\": \"example_value\"\n    },\n    \"record_link\": {\n      \"type\": \"string\",\n      \"description\": \"A link to the target record in\
  \ ServiceNow.\",\n      \"format\": \"uri\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The transformation status. Common values include inserted, updated, error, and ignored.\",\n      \"example\": \"inserted\",\n      \"enum\": [\n        \"inserted\",\n        \"updated\",\n        \"error\",\n        \"ignored\"\n      ]\n    },\n    \"status_message\": {\n      \"type\": \"string\",\n      \"description\": \"A descriptive message about the transformation result, especially useful when the status is error.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the import set row record in the staging table.\",\n      \"example\": \"500123\"\n    },\n    \"target_sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the record created or updated in the target table.\",\n      \"example\": \"\
  500123\"\n    },\n    \"import_set\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the parent import set.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImportSetResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-import-set-import-set-result-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: ImportSetResult
---
