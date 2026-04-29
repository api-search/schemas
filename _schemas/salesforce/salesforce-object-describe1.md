---
description: ''
layout: schema
name: ObjectDescribe1
properties_list:
- description: ''
  name: activateable
  type: boolean
- description: ''
  name: associateEntityType
  type: '[''string'', ''null'']'
- description: ''
  name: associateParentEntity
  type: '[''string'', ''null'']'
- description: ''
  name: createable
  type: boolean
- description: ''
  name: custom
  type: boolean
- description: ''
  name: customSetting
  type: boolean
- description: ''
  name: deepCloneable
  type: boolean
- description: ''
  name: deletable
  type: boolean
- description: ''
  name: deprecatedAndHidden
  type: boolean
- description: ''
  name: feedEnabled
  type: boolean
- description: ''
  name: hasSubtypes
  type: boolean
- description: ''
  name: isInterface
  type: boolean
- description: ''
  name: isSubtype
  type: boolean
- description: ''
  name: keyPrefix
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: labelPlural
  type: string
- description: ''
  name: layoutable
  type: boolean
- description: ''
  name: mergeable
  type: boolean
- description: ''
  name: mruEnabled
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: queryable
  type: boolean
- description: ''
  name: replicateable
  type: boolean
- description: ''
  name: retrieveable
  type: boolean
- description: ''
  name: searchable
  type: boolean
- description: ''
  name: triggerable
  type: boolean
- description: ''
  name: undeletable
  type: boolean
- description: ''
  name: updateable
  type: boolean
- description: ''
  name: urls
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-object-describe1-schema.json
slug: salesforce-object-describe1
source_filename: salesforce-object-describe1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"activateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"associateEntityType\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"associateParentEntity\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"custom\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"customSetting\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deepCloneable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deletable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deprecatedAndHidden\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"feedEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n\
  \    \"hasSubtypes\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isInterface\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isSubtype\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"keyPrefix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"labelPlural\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"layoutable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"mergeable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"mruEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"queryable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"replicateable\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"retrieveable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"searchable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"triggerable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"undeletable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"compactLayouts\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"rowTemplate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"describe\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"layouts\": {\n          \"type\": \"string\",\n          \"example\": \"\
  example_value\"\n        },\n        \"sobject\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"compactLayouts\",\n        \"rowTemplate\",\n        \"describe\",\n        \"layouts\",\n        \"sobject\"\n      ]\n    }\n  },\n  \"required\": [\n    \"activateable\",\n    \"associateEntityType\",\n    \"associateParentEntity\",\n    \"createable\",\n    \"custom\",\n    \"customSetting\",\n    \"deepCloneable\",\n    \"deletable\",\n    \"deprecatedAndHidden\",\n    \"feedEnabled\",\n    \"hasSubtypes\",\n    \"isInterface\",\n    \"isSubtype\",\n    \"keyPrefix\",\n    \"label\",\n    \"labelPlural\",\n    \"layoutable\",\n    \"mergeable\",\n    \"mruEnabled\",\n    \"name\",\n    \"queryable\",\n    \"replicateable\",\n    \"retrieveable\",\n    \"searchable\",\n    \"triggerable\",\n    \"undeletable\",\n    \"updateable\",\n    \"urls\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ObjectDescribe1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-object-describe1-schema.json
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
title: ObjectDescribe1
---
