---
description: A CloudStack virtual machine resource with its configuration and runtime state.
layout: schema
name: VirtualMachine
properties_list:
- description: UUID of the virtual machine.
  name: id
  type: string
- description: Display name of the virtual machine.
  name: name
  type: string
- description: Current state of the virtual machine.
  name: state
  type: string
- description: UUID of the zone containing the virtual machine.
  name: zoneid
  type: string
- description: Name of the zone containing the virtual machine.
  name: zonename
  type: string
- description: UUID of the service offering used by the virtual machine.
  name: serviceofferingid
  type: string
- description: UUID of the template used to create the virtual machine.
  name: templateid
  type: string
- description: Number of CPU cores.
  name: cpunumber
  type: integer
- description: Memory in megabytes.
  name: memory
  type: integer
- description: Primary IP address of the virtual machine.
  name: ipaddress
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-virtual-machine-schema.json
slug: cloudstack-api-virtual-machine
source_filename: cloudstack-api-virtual-machine-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-virtual-machine-schema.json\",\n  \"title\": \"VirtualMachine\",\n  \"description\": \"A CloudStack virtual machine resource with its configuration and runtime state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"UUID of the virtual machine.\", \"example\": \"vm-uuid-1234\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Display name of the virtual machine.\", \"example\": \"web-server-01\" },\n    \"state\": { \"type\": \"string\", \"description\": \"Current state of the virtual machine.\", \"enum\": [\"Running\", \"Stopped\", \"Starting\", \"Stopping\", \"Destroyed\", \"Expunging\", \"Migrating\", \"Error\"], \"example\": \"Running\" },\n    \"zoneid\": { \"type\": \"string\", \"description\": \"UUID of the zone\
  \ containing the virtual machine.\", \"example\": \"zone-uuid-abcd\" },\n    \"zonename\": { \"type\": \"string\", \"description\": \"Name of the zone containing the virtual machine.\", \"example\": \"us-east-1\" },\n    \"serviceofferingid\": { \"type\": \"string\", \"description\": \"UUID of the service offering used by the virtual machine.\", \"example\": \"so-uuid-5678\" },\n    \"templateid\": { \"type\": \"string\", \"description\": \"UUID of the template used to create the virtual machine.\", \"example\": \"tmpl-uuid-9012\" },\n    \"cpunumber\": { \"type\": \"integer\", \"description\": \"Number of CPU cores.\", \"example\": 2 },\n    \"memory\": { \"type\": \"integer\", \"description\": \"Memory in megabytes.\", \"example\": 2048 },\n    \"ipaddress\": { \"type\": \"string\", \"description\": \"Primary IP address of the virtual machine.\", \"example\": \"10.0.0.100\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-virtual-machine-schema.json
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: VirtualMachine
---
