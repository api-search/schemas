---
description: ''
layout: schema
name: UserPermissionsWorkDotComUserFeature
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: calculated
  type: boolean
- description: ''
  name: compound
  type: boolean
- description: ''
  name: compoundComponentName
  type: '[''string'', ''null'']'
- description: ''
  name: compoundFieldName
  type: '[''string'', ''null'']'
- description: ''
  name: controllerName
  type: '[''string'', ''null'']'
- description: ''
  name: controllingFields
  type: array
- description: ''
  name: createable
  type: boolean
- description: ''
  name: custom
  type: boolean
- description: ''
  name: dataType
  type: string
- description: ''
  name: extraTypeInfo
  type: '[''string'', ''null'']'
- description: ''
  name: filterable
  type: boolean
- description: ''
  name: filteredLookupInfo
  type: '[''string'', ''null'']'
- description: ''
  name: highScaleNumber
  type: boolean
- description: ''
  name: htmlFormatted
  type: boolean
- description: ''
  name: inlineHelpText
  type: '[''string'', ''null'']'
- description: ''
  name: label
  type: string
- description: ''
  name: length
  type: integer
- description: ''
  name: nameField
  type: boolean
- description: ''
  name: polymorphicForeignKey
  type: boolean
- description: ''
  name: precision
  type: integer
- description: ''
  name: reference
  type: boolean
- description: ''
  name: referenceTargetField
  type: '[''string'', ''null'']'
- description: ''
  name: referenceToInfos
  type: array
- description: ''
  name: relationshipName
  type: '[''string'', ''null'']'
- description: ''
  name: required
  type: boolean
- description: ''
  name: scale
  type: integer
- description: ''
  name: searchPrefilterable
  type: boolean
- description: ''
  name: sortable
  type: boolean
- description: ''
  name: unique
  type: boolean
- description: ''
  name: updateable
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-user-permissions-work-dot-com-user-feature-schema.json
slug: salesforce-user-permissions-work-dot-com-user-feature
source_filename: salesforce-user-permissions-work-dot-com-user-feature-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"calculated\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"compound\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"compoundComponentName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"compoundFieldName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"controllerName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"controllingFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"custom\": {\n      \"type\": \"boolean\",\n      \"\
  example\": true\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"extraTypeInfo\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"filterable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"filteredLookupInfo\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"highScaleNumber\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"htmlFormatted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"inlineHelpText\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"nameField\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"polymorphicForeignKey\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"precision\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"reference\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"referenceTargetField\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"referenceToInfos\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"relationshipName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"scale\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"searchPrefilterable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"sortable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"unique\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"apiName\",\n    \"calculated\",\n    \"compound\",\n    \"compoundComponentName\",\n    \"compoundFieldName\",\n    \"controllerName\",\n    \"controllingFields\",\n    \"createable\",\n    \"custom\",\n    \"dataType\",\n    \"extraTypeInfo\",\n    \"filterable\",\n    \"filteredLookupInfo\",\n    \"highScaleNumber\",\n    \"htmlFormatted\",\n    \"inlineHelpText\",\n    \"label\",\n    \"length\",\n    \"nameField\",\n    \"polymorphicForeignKey\",\n    \"precision\",\n    \"reference\",\n    \"referenceTargetField\",\n    \"referenceToInfos\",\n    \"relationshipName\",\n    \"required\",\n    \"scale\",\n    \"searchPrefilterable\",\n    \"sortable\",\n    \"unique\",\n    \"updateable\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserPermissionsWorkDotComUserFeature\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-user-permissions-work-dot-com-user-feature-schema.json
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
title: UserPermissionsWorkDotComUserFeature
---
