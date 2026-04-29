---
description: A node pool in a Kubernetes cluster.
layout: schema
name: NodePool
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: clusterId
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: kubernetesVersion
  type: string
- description: ''
  name: nodeShape
  type: string
- description: ''
  name: quantityPerSubnet
  type: integer
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/oke-node-pool-schema.json
slug: oke-node-pool
source_filename: oke-node-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-node-pool-schema.json\",\n  \"title\": \"NodePool\",\n  \"description\": \"A node pool in a Kubernetes cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"pool1\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v1.28.2\"\n    },\n    \"nodeShape\": {\n      \"type\": \"string\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"\
  quantityPerSubnet\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-node-pool-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: NodePool
---
