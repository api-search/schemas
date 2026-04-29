---
description: Information about a SASE service affected by a notification.
layout: schema
name: ServiceInfo
properties_list:
- description: Name of the SASE service.
  name: serviceName
  type: string
- description: Current operational status of the service.
  name: serviceStatus
  type: string
- description: Region where the service is deployed.
  name: region
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-service-info-schema.json
slug: sase-notifications-service-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceInfo\",\n  \"description\": \"Information about a SASE service affected by a notification.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-service-info-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SASE service.\"\n    },\n    \"serviceStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"operational\",\n        \"degraded\",\n        \"maintenance\",\n        \"outage\"\n      ],\n      \"description\": \"Current operational status of the service.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region where the service is deployed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-service-info-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceInfo
---
