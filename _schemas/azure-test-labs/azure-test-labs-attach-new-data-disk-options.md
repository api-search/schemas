---
description: Properties to attach new disk to the Virtual Machine.
layout: schema
name: AttachNewDataDiskOptions
properties_list:
- description: The name of the disk to be attached.
  name: diskName
  type: string
- description: Size of the disk to be attached in GibiBytes.
  name: diskSizeGiB
  type: integer
- description: The storage type for the disk (i.e. Standard, Premium).
  name: diskType
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-attach-new-data-disk-options-schema.json
slug: azure-test-labs-attach-new-data-disk-options
source_filename: azure-test-labs-attach-new-data-disk-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-attach-new-data-disk-options-schema.json\",\n  \"title\": \"AttachNewDataDiskOptions\",\n  \"description\": \"Properties to attach new disk to the Virtual Machine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"diskName\": {\n      \"description\": \"The name of the disk to be attached.\",\n      \"type\": \"string\"\n    },\n    \"diskSizeGiB\": {\n      \"description\": \"Size of the disk to be attached in GibiBytes.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"diskType\": {\n      \"description\": \"The storage type for the disk (i.e. Standard, Premium).\",\n      \"enum\": [\n        \"Standard\",\n        \"Premium\",\n        \"StandardSSD\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n \
  \       \"name\": \"StorageType\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-attach-new-data-disk-options-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: AttachNewDataDiskOptions
---
