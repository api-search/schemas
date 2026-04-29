---
description: A node in the ONTAP cluster
layout: schema
name: ClusterNode
properties_list:
- description: Node UUID
  name: uuid
  type: string
- description: Node name
  name: name
  type: string
- description: Hardware model of the node
  name: model
  type: string
- description: System serial number
  name: serial_number
  type: string
- description: Node uptime in seconds
  name: uptime
  type: integer
- description: ONTAP version running on the node
  name: version
  type: object
- description: Node controller information
  name: controller
  type: object
- description: Current operational state of the node
  name: state
  type: string
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-cluster-node-schema.json
slug: netapp-ontap-cluster-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterNode\",\n  \"type\": \"object\",\n  \"description\": \"A node in the ONTAP cluster\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Node UUID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Node name\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model of the node\"\n    },\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"System serial number\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Node uptime in seconds\"\n    },\n    \"version\": {\n      \"type\": \"object\",\n      \"description\": \"ONTAP version running on the node\"\n    },\n    \"controller\": {\n      \"type\": \"object\",\n      \"description\": \"Node controller information\"\n    },\n    \"state\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Current operational state of the node\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-cluster-node-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: ClusterNode
---
