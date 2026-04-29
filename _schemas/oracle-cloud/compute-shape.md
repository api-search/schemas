---
description: A compute shape defining the resources available for an instance.
layout: schema
name: Shape
properties_list:
- description: The name of the shape.
  name: shape
  type: string
- description: Description of the processor.
  name: processorDescription
  type: string
- description: Default number of OCPUs.
  name: ocpus
  type: number
- description: Default amount of memory in gigabytes.
  name: memoryInGBs
  type: number
- description: Number of GPUs.
  name: gpus
  type: integer
- description: Networking bandwidth in Gbps.
  name: networkingBandwidthInGbps
  type: number
- description: Whether the shape is flexible.
  name: isFlexible
  type: boolean
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-shape-schema.json
slug: compute-shape
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-shape-schema.json\",\n  \"title\": \"Shape\",\n  \"description\": \"A compute shape defining the resources available for an instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shape\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the shape.\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"processorDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the processor.\",\n      \"example\": \"2.55 GHz AMD EPYC 7J13\"\n    },\n    \"ocpus\": {\n      \"type\": \"number\",\n      \"description\": \"Default number of OCPUs.\",\n      \"example\": \"1.0\"\n    },\n    \"memoryInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"Default amount of memory in gigabytes.\",\n      \"example\": \"16.0\"\n    },\n \
  \   \"gpus\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of GPUs.\",\n      \"example\": \"0\"\n    },\n    \"networkingBandwidthInGbps\": {\n      \"type\": \"number\",\n      \"description\": \"Networking bandwidth in Gbps.\",\n      \"example\": \"1.0\"\n    },\n    \"isFlexible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the shape is flexible.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-shape-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Shape
---
