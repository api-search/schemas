---
description: A load balancer probe.
layout: schema
name: Probe
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within the set of probes used by the load balancer. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of load balancer probe.
  name: properties
  type: object
- description: Type of the resource.
  name: type
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-probe-schema.json
slug: azure-networking-services-probe
source_filename: azure-networking-services-probe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-probe-schema.json\",\n  \"title\": \"Probe\",\n  \"description\": \"A load balancer probe.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the resource that is unique within the set of probes used by the load balancer. This name can be used to access the resource.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/ProbePropertiesFormat\",\n      \"description\": \"Properties of load balancer probe.\",\n      \"x-ms-client-flatten\": true\n    },\n    \"type\": {\n      \"description\": \"Type of the resource.\",\n      \"readOnly\": true,\n\
  \      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-probe-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: Probe
---
