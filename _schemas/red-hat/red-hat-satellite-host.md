---
description: A host managed by Red Hat Satellite.
layout: schema
name: Host
properties_list:
- description: The unique identifier of the host.
  name: id
  type: integer
- description: The fully qualified domain name of the host.
  name: name
  type: string
- description: The IP address of the host.
  name: ip
  type: string
- description: The MAC address of the primary interface.
  name: mac
  type: string
- description: The operating system name and version.
  name: operatingsystem_name
  type: string
- description: The Puppet environment name.
  name: environment_name
  type: string
- description: The host group name.
  name: hostgroup_name
  type: string
- description: The organization name.
  name: organization_name
  type: string
- description: The location name.
  name: location_name
  type: string
- description: The global host status (0=OK, 1=Warning, 2=Error).
  name: global_status
  type: integer
- description: Content-related attributes of the host.
  name: content_facet_attributes
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-satellite-host-schema.json
slug: red-hat-satellite-host
source_filename: red-hat-satellite-host-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Host\",\n  \"type\": \"object\",\n  \"description\": \"A host managed by Red Hat Satellite.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the host.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified domain name of the host.\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address of the host.\"\n    },\n    \"mac\": {\n      \"type\": \"string\",\n      \"description\": \"The MAC address of the primary interface.\"\n    },\n    \"operatingsystem_name\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system name and version.\"\n    },\n    \"environment_name\": {\n      \"type\": \"string\",\n      \"description\": \"The Puppet environment name.\"\n    },\n    \"hostgroup_name\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The host group name.\"\n    },\n    \"organization_name\": {\n      \"type\": \"string\",\n      \"description\": \"The organization name.\"\n    },\n    \"location_name\": {\n      \"type\": \"string\",\n      \"description\": \"The location name.\"\n    },\n    \"global_status\": {\n      \"type\": \"integer\",\n      \"description\": \"The global host status (0=OK, 1=Warning, 2=Error).\"\n    },\n    \"content_facet_attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Content-related attributes of the host.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-satellite-host-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Host
---
