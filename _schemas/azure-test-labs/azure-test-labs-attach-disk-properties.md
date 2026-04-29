---
description: Properties of the disk to attach.
layout: schema
name: AttachDiskProperties
properties_list:
- description: The resource ID of the Lab virtual machine to which the disk is attached.
  name: leasedByLabVmId
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-attach-disk-properties-schema.json
slug: azure-test-labs-attach-disk-properties
source_filename: azure-test-labs-attach-disk-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-attach-disk-properties-schema.json\",\n  \"title\": \"AttachDiskProperties\",\n  \"description\": \"Properties of the disk to attach.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"leasedByLabVmId\": {\n      \"description\": \"The resource ID of the Lab virtual machine to which the disk is attached.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-attach-disk-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: AttachDiskProperties
---
