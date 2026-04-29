---
description: Properties of an Azure Resource Manager template.
layout: schema
name: ArmTemplateProperties
properties_list:
- description: The contents of the ARM template.
  name: contents
  type: object
- description: The creation date of the armTemplate.
  name: createdDate
  type: string
- description: The description of the ARM template.
  name: description
  type: string
- description: The display name of the ARM template.
  name: displayName
  type: string
- description: Whether or not ARM template is enabled for use by lab user.
  name: enabled
  type: boolean
- description: The URI to the icon of the ARM template.
  name: icon
  type: string
- description: File name and parameter values information from all azuredeploy.*.parameters.json for the ARM template.
  name: parametersValueFilesInfo
  type: array
- description: The publisher of the ARM template.
  name: publisher
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-arm-template-properties-schema.json
slug: azure-test-labs-arm-template-properties
source_filename: azure-test-labs-arm-template-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-properties-schema.json\",\n  \"title\": \"ArmTemplateProperties\",\n  \"description\": \"Properties of an Azure Resource Manager template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contents\": {\n      \"description\": \"The contents of the ARM template.\",\n      \"readOnly\": true,\n      \"type\": \"object\"\n    },\n    \"createdDate\": {\n      \"description\": \"The creation date of the armTemplate.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"The description of the ARM template.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"The display name of the ARM template.\",\n      \"readOnly\"\
  : true,\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"description\": \"Whether or not ARM template is enabled for use by lab user.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"icon\": {\n      \"description\": \"The URI to the icon of the ARM template.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"parametersValueFilesInfo\": {\n      \"description\": \"File name and parameter values information from all azuredeploy.*.parameters.json for the ARM template.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ParametersValueFileInfo\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"publisher\": {\n      \"description\": \"The publisher of the ARM template.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArmTemplateProperties
---
