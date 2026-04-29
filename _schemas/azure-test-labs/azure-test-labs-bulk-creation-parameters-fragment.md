---
description: Parameters for creating multiple virtual machines as a single action.
layout: schema
name: BulkCreationParametersFragment
properties_list:
- description: The number of virtual machine instances to create.
  name: instanceCount
  type: integer
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-bulk-creation-parameters-fragment-schema.json
slug: azure-test-labs-bulk-creation-parameters-fragment
source_filename: azure-test-labs-bulk-creation-parameters-fragment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-bulk-creation-parameters-fragment-schema.json\",\n  \"title\": \"BulkCreationParametersFragment\",\n  \"description\": \"Parameters for creating multiple virtual machines as a single action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceCount\": {\n      \"description\": \"The number of virtual machine instances to create.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-bulk-creation-parameters-fragment-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: BulkCreationParametersFragment
---
