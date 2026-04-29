---
description: The response of a list operation.
layout: schema
name: ArmTemplateList
properties_list:
- description: Link for next set of results.
  name: nextLink
  type: string
- description: Results of the list operation.
  name: value
  type: array
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-arm-template-list-schema.json
slug: azure-test-labs-arm-template-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-list-schema.json\",\n  \"title\": \"ArmTemplateList\",\n  \"description\": \"The response of a list operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"Link for next set of results.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Results of the list operation.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ArmTemplate\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-arm-template-list-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArmTemplateList
---
