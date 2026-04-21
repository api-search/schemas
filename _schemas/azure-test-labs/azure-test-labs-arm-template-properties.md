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
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArmTemplateProperties
---
