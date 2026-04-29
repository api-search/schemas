---
description: ''
layout: schema
name: GetToolingDescribe
properties_list:
- description: ''
  name: encoding
  type: string
- description: ''
  name: maxBatchSize
  type: integer
- description: ''
  name: sobjects
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-tooling-describe-schema.json
slug: salesforce-get-tooling-describe
source_filename: salesforce-get-tooling-describe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"encoding\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"maxBatchSize\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"sobjects\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"activateable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"associateEntityType\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"associateParentEntity\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"createable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"custom\": {\n            \"type\": \"boolean\",\n    \
  \        \"example\": true\n          },\n          \"customSetting\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"deepCloneable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"deletable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"deprecatedAndHidden\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"feedEnabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"hasSubtypes\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"isInterface\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"isSubtype\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"keyPrefix\": {\n            \"type\": \"string\",\n\
  \            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"labelPlural\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"layoutable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"mergeable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"mruEnabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"queryable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"replicateable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"retrieveable\": {\n  \
  \          \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"searchable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"triggerable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"undeletable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"updateable\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"urls\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"rowTemplate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"describe\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"sobject\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\
  \n              }\n            },\n            \"required\": [\n              \"rowTemplate\",\n              \"describe\",\n              \"sobject\"\n            ]\n          }\n        },\n        \"required\": [\n          \"activateable\",\n          \"associateEntityType\",\n          \"associateParentEntity\",\n          \"createable\",\n          \"custom\",\n          \"customSetting\",\n          \"deepCloneable\",\n          \"deletable\",\n          \"deprecatedAndHidden\",\n          \"feedEnabled\",\n          \"hasSubtypes\",\n          \"isInterface\",\n          \"isSubtype\",\n          \"keyPrefix\",\n          \"label\",\n          \"labelPlural\",\n          \"layoutable\",\n          \"mergeable\",\n          \"mruEnabled\",\n          \"name\",\n          \"queryable\",\n          \"replicateable\",\n          \"retrieveable\",\n          \"searchable\",\n          \"triggerable\",\n          \"undeletable\",\n          \"updateable\",\n          \"urls\"\n     \
  \   ]\n      }\n    }\n  },\n  \"required\": [\n    \"encoding\",\n    \"maxBatchSize\",\n    \"sobjects\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetToolingDescribe\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-tooling-describe-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: GetToolingDescribe
---
