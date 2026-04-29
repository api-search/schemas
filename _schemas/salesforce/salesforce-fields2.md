---
description: ''
layout: schema
name: Fields2
properties_list:
- description: ''
  name: aggregatable
  type: boolean
- description: ''
  name: aiPredictionField
  type: boolean
- description: ''
  name: autoNumber
  type: boolean
- description: ''
  name: byteLength
  type: integer
- description: ''
  name: calculated
  type: boolean
- description: ''
  name: calculatedFormula
  type: '[''string'', ''null'']'
- description: ''
  name: cascadeDelete
  type: boolean
- description: ''
  name: caseSensitive
  type: boolean
- description: ''
  name: compoundFieldName
  type: '[''string'', ''null'']'
- description: ''
  name: controllerName
  type: '[''string'', ''null'']'
- description: ''
  name: createable
  type: boolean
- description: ''
  name: custom
  type: boolean
- description: ''
  name: defaultValue
  type: object
- description: ''
  name: defaultValueFormula
  type: '[''string'', ''null'']'
- description: ''
  name: defaultedOnCreate
  type: boolean
- description: ''
  name: dependentPicklist
  type: boolean
- description: ''
  name: deprecatedAndHidden
  type: boolean
- description: ''
  name: digits
  type: integer
- description: ''
  name: displayLocationInDecimal
  type: boolean
- description: ''
  name: encrypted
  type: boolean
- description: ''
  name: externalId
  type: boolean
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
  name: formulaTreatNullNumberAsZero
  type: boolean
- description: ''
  name: groupable
  type: boolean
- description: ''
  name: highScaleNumber
  type: boolean
- description: ''
  name: htmlFormatted
  type: boolean
- description: ''
  name: idLookup
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
  name: mask
  type: '[''string'', ''null'']'
- description: ''
  name: maskType
  type: '[''string'', ''null'']'
- description: ''
  name: name
  type: string
- description: ''
  name: nameField
  type: boolean
- description: ''
  name: namePointing
  type: boolean
- description: ''
  name: nillable
  type: boolean
- description: ''
  name: permissionable
  type: boolean
- description: ''
  name: picklistValues
  type: array
- description: ''
  name: polymorphicForeignKey
  type: boolean
- description: ''
  name: precision
  type: integer
- description: ''
  name: queryByDistance
  type: boolean
- description: ''
  name: referenceTargetField
  type: '[''string'', ''null'']'
- description: ''
  name: referenceTo
  type: array
- description: ''
  name: relationshipName
  type: '[''string'', ''null'']'
- description: ''
  name: relationshipOrder
  type: '[''string'', ''null'']'
- description: ''
  name: restrictedDelete
  type: boolean
- description: ''
  name: restrictedPicklist
  type: boolean
- description: ''
  name: scale
  type: integer
- description: ''
  name: searchPrefilterable
  type: boolean
- description: ''
  name: soapType
  type: string
- description: ''
  name: sortable
  type: boolean
- description: ''
  name: type
  type: string
- description: ''
  name: unique
  type: boolean
- description: ''
  name: updateable
  type: boolean
- description: ''
  name: writeRequiresMasterRead
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-fields2-schema.json
slug: salesforce-fields2
source_filename: salesforce-fields2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregatable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"aiPredictionField\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"autoNumber\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"byteLength\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"calculated\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"calculatedFormula\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"cascadeDelete\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"caseSensitive\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"compoundFieldName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"controllerName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"\
  example_value\"\n    },\n    \"createable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"custom\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"defaultValue\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"defaultValueFormula\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"defaultedOnCreate\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"dependentPicklist\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"deprecatedAndHidden\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"digits\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"displayLocationInDecimal\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"externalId\": {\n      \"type\": \"\
  boolean\",\n      \"example\": \"500123\"\n    },\n    \"extraTypeInfo\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"filterable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"filteredLookupInfo\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"formulaTreatNullNumberAsZero\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"groupable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"highScaleNumber\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"htmlFormatted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"idLookup\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"inlineHelpText\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"Example Title\"\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"mask\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"maskType\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"nameField\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"namePointing\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"nillable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"permissionable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"picklistValues\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"polymorphicForeignKey\": {\n      \"type\": \"boolean\",\n\
  \      \"example\": true\n    },\n    \"precision\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"queryByDistance\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"referenceTargetField\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"referenceTo\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"relationshipName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"relationshipOrder\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"restrictedDelete\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"restrictedPicklist\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"scale\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n\
  \    \"searchPrefilterable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"soapType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sortable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"unique\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updateable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"writeRequiresMasterRead\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"aggregatable\",\n    \"aiPredictionField\",\n    \"autoNumber\",\n    \"byteLength\",\n    \"calculated\",\n    \"calculatedFormula\",\n    \"cascadeDelete\",\n    \"caseSensitive\",\n    \"compoundFieldName\",\n    \"controllerName\",\n    \"createable\",\n    \"custom\",\n    \"defaultValue\",\n    \"defaultValueFormula\",\n    \"\
  defaultedOnCreate\",\n    \"dependentPicklist\",\n    \"deprecatedAndHidden\",\n    \"digits\",\n    \"displayLocationInDecimal\",\n    \"encrypted\",\n    \"externalId\",\n    \"extraTypeInfo\",\n    \"filterable\",\n    \"filteredLookupInfo\",\n    \"formulaTreatNullNumberAsZero\",\n    \"groupable\",\n    \"highScaleNumber\",\n    \"htmlFormatted\",\n    \"idLookup\",\n    \"inlineHelpText\",\n    \"label\",\n    \"length\",\n    \"mask\",\n    \"maskType\",\n    \"name\",\n    \"nameField\",\n    \"namePointing\",\n    \"nillable\",\n    \"permissionable\",\n    \"picklistValues\",\n    \"polymorphicForeignKey\",\n    \"precision\",\n    \"queryByDistance\",\n    \"referenceTargetField\",\n    \"referenceTo\",\n    \"relationshipName\",\n    \"relationshipOrder\",\n    \"restrictedDelete\",\n    \"restrictedPicklist\",\n    \"scale\",\n    \"searchPrefilterable\",\n    \"soapType\",\n    \"sortable\",\n    \"type\",\n    \"unique\",\n    \"updateable\",\n    \"writeRequiresMasterRead\"\
  \n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fields2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-fields2-schema.json
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
title: Fields2
---
