---
description: Binding between a content switching virtual server and a content switching policy. Defines how requests are evaluated and routed to target load balancing virtual servers.
layout: schema
name: CsVserverCsPolicyBinding
properties_list:
- description: Name of the content switching virtual server.
  name: name
  type: string
- description: Name of the content switching policy to bind.
  name: policyname
  type: string
- description: Name of the target load balancing virtual server to which matching traffic is directed.
  name: targetlbvserver
  type: string
- description: Priority of the policy binding. Lower values indicate higher priority.
  name: priority
  type: integer
- description: Expression specifying the priority of the next policy to evaluate if the current policy matches.
  name: gotopriorityexpression
  type: string
- description: The bind point at which the policy is bound.
  name: bindpoint
  type: string
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-cs-vserver-cs-policy-binding-schema.json
slug: citrix-netscaler-nitro-cs-vserver-cs-policy-binding
source_filename: citrix-netscaler-nitro-cs-vserver-cs-policy-binding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CsVserverCsPolicyBinding\",\n  \"type\": \"object\",\n  \"description\": \"Binding between a content switching virtual server and a content switching policy. Defines how requests are evaluated and routed to target load balancing virtual servers.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content switching virtual server.\"\n    },\n    \"policyname\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content switching policy to bind.\"\n    },\n    \"targetlbvserver\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target load balancing virtual server to which matching traffic is directed.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the policy binding. Lower values indicate higher priority.\"\n    },\n    \"gotopriorityexpression\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Expression specifying the priority of the next policy to evaluate if the current policy matches.\"\n    },\n    \"bindpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The bind point at which the policy is bound.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-cs-vserver-cs-policy-binding-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: CsVserverCsPolicyBinding
---
