---
description: AgentNetworkInfo schema from Amazon Application Discovery Service API
layout: schema
name: AgentNetworkInfo
properties_list:
- description: The IP address for the host where the agent or collector resides.
  name: ipAddress
  type: string
- description: The MAC address for the host where the agent or collector resides.
  name: macAddress
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-agent-network-info-schema.json
slug: application-discovery-service-agent-network-info
source_filename: application-discovery-service-agent-network-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-agent-network-info-schema.json\",\n  \"title\": \"AgentNetworkInfo\",\n  \"description\": \"AgentNetworkInfo schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"example\": \"10.0.0.10\",\n      \"description\": \"The IP address for the host where the agent or collector resides.\"\n    },\n    \"macAddress\": {\n      \"type\": \"string\",\n      \"example\": \"aa:bb:cc:dd:ee:ff\",\n      \"description\": \"The MAC address for the host where the agent or collector resides.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-agent-network-info-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: AgentNetworkInfo
---
