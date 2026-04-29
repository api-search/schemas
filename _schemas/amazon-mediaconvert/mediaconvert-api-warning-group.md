---
description: Contains any warning codes and their count for the job.
layout: schema
name: WarningGroup
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: Count
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-warning-group-schema.json
slug: mediaconvert-api-warning-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-warning-group-schema.json\",\n  \"title\": \"WarningGroup\",\n  \"description\": \"Contains any warning codes and their count for the job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"code\"\n          },\n          \"description\": \"Warning code that identifies a specific warning in the job. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/warning_codes.html\"\n        }\n      ]\n    },\n    \"Count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"count\"\n        \
  \  },\n          \"description\": \"The number of times this warning occurred in the job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Count\",\n    \"Code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-warning-group-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: WarningGroup
---
