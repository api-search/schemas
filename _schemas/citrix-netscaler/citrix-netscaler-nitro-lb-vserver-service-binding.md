---
description: Binding between a load balancing virtual server and a backend service. This allows the virtual server to distribute traffic to the bound service.
layout: schema
name: LbVserverServiceBinding
properties_list:
- description: Name of the load balancing virtual server to which the service is bound.
  name: name
  type: string
- description: Name of the service to bind to the virtual server.
  name: servicename
  type: string
- description: Weight assigned to the service for weighted load balancing. Range 1-100.
  name: weight
  type: integer
- description: Protocol type of the bound service.
  name: servicetype
  type: string
- description: Current state of the bound service.
  name: curstate
  type: string
- description: IP address of the bound service.
  name: ipv46
  type: string
- description: Port of the bound service.
  name: port
  type: integer
- description: Dynamic weight of the service based on server health.
  name: dynamicweight
  type: integer
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-lb-vserver-service-binding-schema.json
slug: citrix-netscaler-nitro-lb-vserver-service-binding
source_filename: citrix-netscaler-nitro-lb-vserver-service-binding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LbVserverServiceBinding\",\n  \"type\": \"object\",\n  \"description\": \"Binding between a load balancing virtual server and a backend service. This allows the virtual server to distribute traffic to the bound service.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the load balancing virtual server to which the service is bound.\"\n    },\n    \"servicename\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service to bind to the virtual server.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight assigned to the service for weighted load balancing. Range 1-100.\"\n    },\n    \"servicetype\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol type of the bound service.\"\n    },\n    \"curstate\": {\n      \"type\": \"string\",\n      \"description\": \"Current\
  \ state of the bound service.\"\n    },\n    \"ipv46\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the bound service.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port of the bound service.\"\n    },\n    \"dynamicweight\": {\n      \"type\": \"integer\",\n      \"description\": \"Dynamic weight of the service based on server health.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-lb-vserver-service-binding-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: LbVserverServiceBinding
---
