---
description: Options for configuring networking bandwidth on a flexible shape
layout: schema
name: ShapeNetworkingBandwidthOptions
properties_list:
- description: The minimum networking bandwidth, in Gbps
  name: minInGbps
  type: number
- description: The maximum networking bandwidth, in Gbps
  name: maxInGbps
  type: number
- description: The default networking bandwidth per OCPU, in Gbps
  name: defaultPerOcpuInGbps
  type: number
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-shape-networking-bandwidth-options-schema.json
slug: oci-compute-shape-networking-bandwidth-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShapeNetworkingBandwidthOptions\",\n  \"type\": \"object\",\n  \"description\": \"Options for configuring networking bandwidth on a flexible shape\",\n  \"properties\": {\n    \"minInGbps\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum networking bandwidth, in Gbps\"\n    },\n    \"maxInGbps\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum networking bandwidth, in Gbps\"\n    },\n    \"defaultPerOcpuInGbps\": {\n      \"type\": \"number\",\n      \"description\": \"The default networking bandwidth per OCPU, in Gbps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-shape-networking-bandwidth-options-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: ShapeNetworkingBandwidthOptions
---
