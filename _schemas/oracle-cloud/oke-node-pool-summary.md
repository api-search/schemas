---
description: NodePoolSummary schema from oracle-cloud-oke-openapi.yaml
layout: schema
name: NodePoolSummary
properties_list:
- description: ''
  name: id
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
  name: lifecycleState
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/oke-node-pool-summary-schema.json
slug: oke-node-pool-summary
source_filename: oke-node-pool-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-node-pool-summary-schema.json\",\n  \"title\": \"NodePoolSummary\",\n  \"description\": \"NodePoolSummary schema from oracle-cloud-oke-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v1.28.2\"\n    },\n    \"nodeShape\": {\n      \"type\": \"string\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-node-pool-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: NodePoolSummary
---
