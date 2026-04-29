---
description: Status information for a Host resource
layout: schema
name: HostStatus
properties_list:
- description: Current state of the Host
  name: state
  type: string
- description: Last completed phase of the Host lifecycle
  name: phaseCompleted
  type: string
- description: Description of any error state
  name: errorReason
  type: string
- description: Source of the TLS certificate
  name: tlsCertificateSource
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-host-status-schema.json
slug: ambassador-host-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status information for a Host resource\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the Host\"\n    },\n    \"phaseCompleted\": {\n      \"type\": \"string\",\n      \"description\": \"Last completed phase of the Host lifecycle\"\n    },\n    \"errorReason\": {\n      \"type\": \"string\",\n      \"description\": \"Description of any error state\"\n    },\n    \"tlsCertificateSource\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the TLS certificate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-host-status-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: HostStatus
---
