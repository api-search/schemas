---
description: Options for configuring OCPUs on a flexible shape
layout: schema
name: ShapeOcpuOptions
properties_list:
- description: The minimum number of OCPUs
  name: min
  type: number
- description: The maximum number of OCPUs
  name: max
  type: number
- description: The maximum number of OCPUs per NUMA node
  name: maxPerNumaNode
  type: number
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-shape-ocpu-options-schema.json
slug: oci-compute-shape-ocpu-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShapeOcpuOptions\",\n  \"type\": \"object\",\n  \"description\": \"Options for configuring OCPUs on a flexible shape\",\n  \"properties\": {\n    \"min\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum number of OCPUs\"\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum number of OCPUs\"\n    },\n    \"maxPerNumaNode\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum number of OCPUs per NUMA node\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-shape-ocpu-options-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: ShapeOcpuOptions
---
