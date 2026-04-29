---
description: A batch job identifier in which the batch job to run is identified by the script name.
layout: schema
name: ScriptBatchJobIdentifier
properties_list:
- description: ''
  name: scriptName
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-script-batch-job-identifier-schema.json
slug: amazon-mainframe-modernization-script-batch-job-identifier
source_filename: amazon-mainframe-modernization-script-batch-job-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-script-batch-job-identifier-schema.json\",\n  \"title\": \"ScriptBatchJobIdentifier\",\n  \"description\": \"A batch job identifier in which the batch job to run is identified by the script name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scriptName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the script containing the batch job definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"scriptName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-script-batch-job-identifier-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ScriptBatchJobIdentifier
---
