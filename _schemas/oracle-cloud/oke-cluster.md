---
description: A Kubernetes cluster managed by OKE.
layout: schema
name: Cluster
properties_list:
- description: The OCID of the cluster.
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
  name: vcnId
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: endpoints
  type: object
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/oke-cluster-schema.json
slug: oke-cluster
source_filename: oke-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"A Kubernetes cluster managed by OKE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the cluster.\",\n      \"example\": \"ocid1.cluster.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my-cluster\"\n    },\n    \"kubernetesVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v1.28.2\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n  \
  \    \"enum\": \"['CREATING', 'ACTIVE', 'FAILED', 'DELETING', 'DELETED', 'UPDATING']\",\n      \"example\": \"CREATING\"\n    },\n    \"endpoints\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"kubernetes\": \"example-value\",\n        \"publicEndpoint\": \"example-value\",\n        \"privateEndpoint\": \"example-value\"\n      }\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/oke-cluster-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Cluster
---
