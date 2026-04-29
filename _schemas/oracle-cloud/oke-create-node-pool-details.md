---
description: CreateNodePoolDetails schema from oracle-cloud-oke-openapi.yaml
layout: schema
name: CreateNodePoolDetails
properties_list:
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: clusterId
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
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/oke-create-node-pool-details-schema.json
slug: oke-create-node-pool-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-create-node-pool-details-schema.json\",\n  \"title\": \"CreateNodePoolDetails\",\n  \"description\": \"CreateNodePoolDetails schema from oracle-cloud-oke-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"clusterId\",\n    \"name\",\n    \"kubernetesVersion\",\n    \"nodeShape\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v1.28.2\"\n    },\n    \"nodeShape\": {\n      \"\
  type\": \"string\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"quantityPerSubnet\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-create-node-pool-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateNodePoolDetails
---
