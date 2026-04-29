---
description: Information about a generated ARM template.
layout: schema
name: ArmTemplateInfo
properties_list:
- description: The parameters of the ARM template.
  name: parameters
  type: object
- description: The template's contents.
  name: template
  type: object
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-arm-template-info-schema.json
slug: azure-test-labs-arm-template-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-info-schema.json\",\n  \"title\": \"ArmTemplateInfo\",\n  \"description\": \"Information about a generated ARM template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"description\": \"The parameters of the ARM template.\",\n      \"type\": \"object\"\n    },\n    \"template\": {\n      \"description\": \"The template's contents.\",\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-info-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArmTemplateInfo
---
