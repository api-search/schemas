---
description: A CloudStack storage volume attached to a virtual machine.
layout: schema
name: Volume
properties_list:
- description: UUID of the volume.
  name: id
  type: string
- description: Display name of the volume.
  name: name
  type: string
- description: Volume type (ROOT or DATADISK).
  name: type
  type: string
- description: Current state of the volume.
  name: state
  type: string
- description: Volume size in bytes.
  name: size
  type: integer
- description: UUID of the virtual machine this volume is attached to.
  name: virtualmachineid
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-volume-schema.json
slug: cloudstack-api-volume
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-volume-schema.json\",\n  \"title\": \"Volume\",\n  \"description\": \"A CloudStack storage volume attached to a virtual machine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"UUID of the volume.\", \"example\": \"vol-uuid-1234\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Display name of the volume.\", \"example\": \"ROOT-1234\" },\n    \"type\": { \"type\": \"string\", \"description\": \"Volume type (ROOT or DATADISK).\", \"enum\": [\"ROOT\", \"DATADISK\"], \"example\": \"ROOT\" },\n    \"state\": { \"type\": \"string\", \"description\": \"Current state of the volume.\", \"example\": \"Ready\" },\n    \"size\": { \"type\": \"integer\", \"format\": \"int64\", \"description\": \"Volume size in bytes.\", \"example\"\
  : 53687091200 },\n    \"virtualmachineid\": { \"type\": \"string\", \"description\": \"UUID of the virtual machine this volume is attached to.\", \"example\": \"vm-uuid-1234\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-volume-schema.json
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: Volume
---
