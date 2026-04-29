---
description: An Azure Resource Manager template.
layout: schema
name: ArmTemplate
properties_list:
- description: The properties of the resource.
  name: properties
  type: object
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-arm-template-schema.json
slug: azure-test-labs-arm-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-schema.json\",\n  \"title\": \"ArmTemplate\",\n  \"description\": \"An Azure Resource Manager template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ArmTemplateProperties\",\n      \"description\": \"The properties of the resource.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArmTemplate
---
