---
description: Response for ListProbe API service call.
layout: schema
name: LoadBalancerProbeListResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: A list of probes in a load balancer.
  name: value
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancer-probe-list-result-schema.json
slug: azure-networking-services-load-balancer-probe-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-probe-list-result-schema.json\",\n  \"title\": \"LoadBalancerProbeListResult\",\n  \"description\": \"Response for ListProbe API service call.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"A list of probes in a load balancer.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Probe\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-probe-list-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancerProbeListResult
---
