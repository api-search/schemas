---
description: Options for configuring memory on a flexible shape
layout: schema
name: ShapeMemoryOptions
properties_list:
- description: The minimum amount of memory, in GB
  name: minInGBs
  type: number
- description: The maximum amount of memory, in GB
  name: maxInGBs
  type: number
- description: The default amount of memory per OCPU, in GB
  name: defaultPerOcpuInGBs
  type: number
- description: The minimum amount of memory per OCPU, in GB
  name: minPerOcpuInGBs
  type: number
- description: The maximum amount of memory per OCPU, in GB
  name: maxPerOcpuInGBs
  type: number
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-shape-memory-options-schema.json
slug: oci-compute-shape-memory-options
source_filename: oci-compute-shape-memory-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShapeMemoryOptions\",\n  \"type\": \"object\",\n  \"description\": \"Options for configuring memory on a flexible shape\",\n  \"properties\": {\n    \"minInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum amount of memory, in GB\"\n    },\n    \"maxInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum amount of memory, in GB\"\n    },\n    \"defaultPerOcpuInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The default amount of memory per OCPU, in GB\"\n    },\n    \"minPerOcpuInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum amount of memory per OCPU, in GB\"\n    },\n    \"maxPerOcpuInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum amount of memory per OCPU, in GB\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-shape-memory-options-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: ShapeMemoryOptions
---
