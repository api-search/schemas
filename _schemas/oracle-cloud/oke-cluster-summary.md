---
description: Cluster summary.
layout: schema
name: ClusterSummary
properties_list:
- description: ''
  name: id
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
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/oke-cluster-summary-schema.json
slug: oke-cluster-summary
source_filename: oke-cluster-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-cluster-summary-schema.json\",\n  \"title\": \"ClusterSummary\",\n  \"description\": \"Cluster summary.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v1.28.2\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-cluster-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: ClusterSummary
---
