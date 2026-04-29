---
description: Kubernetes resource requests and limits
layout: schema
name: ResourceRequirements
properties_list:
- description: CPU resource request in Kubernetes units
  name: cpu
  type: string
- description: Memory resource request in Kubernetes units
  name: memory
  type: string
- description: CPU resource limit
  name: cpu_limit
  type: string
- description: Memory resource limit
  name: memory_limit
  type: string
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-resource-requirements-schema.json
slug: platform-services-resource-requirements
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-resource-requirements-schema.json\",\n  \"title\": \"ResourceRequirements\",\n  \"description\": \"Kubernetes resource requests and limits\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpu\": {\n      \"type\": \"string\",\n      \"description\": \"CPU resource request in Kubernetes units\",\n      \"example\": \"500m\"\n    },\n    \"memory\": {\n      \"type\": \"string\",\n      \"description\": \"Memory resource request in Kubernetes units\",\n      \"example\": \"512Mi\"\n    },\n    \"cpu_limit\": {\n      \"type\": \"string\",\n      \"description\": \"CPU resource limit\",\n      \"example\": \"1000m\"\n    },\n    \"memory_limit\": {\n      \"type\": \"string\",\n      \"description\": \"Memory resource limit\",\n      \"example\": \"1Gi\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-resource-requirements-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: ResourceRequirements
---
