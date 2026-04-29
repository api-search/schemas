---
description: Performance statistics for a content switching virtual server.
layout: schema
name: CsVserverStats
properties_list:
- description: Name of the content switching virtual server.
  name: name
  type: string
- description: IP address of the virtual server.
  name: primaryipaddress
  type: string
- description: Port number of the virtual server.
  name: primaryport
  type: integer
- description: Current operational state.
  name: state
  type: string
- description: Number of current client connections.
  name: curclntconnections
  type: number
- description: Number of current server connections.
  name: cursrvrconnections
  type: number
- description: Number of connections in ESTABLISHED state.
  name: establishedconn
  type: number
- description: Total number of virtual server hits.
  name: tothits
  type: number
- description: Rate of hits per second.
  name: hitsrate
  type: number
- description: Total number of requests received.
  name: totalrequests
  type: number
- description: Rate of requests per second.
  name: requestsrate
  type: number
- description: Total number of responses sent.
  name: totalresponses
  type: number
- description: Rate of responses per second.
  name: responsesrate
  type: number
- description: Total bytes of requests received.
  name: totalrequestbytes
  type: number
- description: Total bytes of responses sent.
  name: totalresponsebytes
  type: number
- description: Total packets received.
  name: totalpktsrecvd
  type: number
- description: Total packets sent.
  name: totalpktssent
  type: number
- description: Total spillover events.
  name: totspillovers
  type: number
- description: Total labeled connections.
  name: labelledconn
  type: number
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-cs-vserver-stats-schema.json
slug: citrix-netscaler-nitro-cs-vserver-stats
source_filename: citrix-netscaler-nitro-cs-vserver-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CsVserverStats\",\n  \"type\": \"object\",\n  \"description\": \"Performance statistics for a content switching virtual server.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content switching virtual server.\"\n    },\n    \"primaryipaddress\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the virtual server.\"\n    },\n    \"primaryport\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number of the virtual server.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state.\"\n    },\n    \"curclntconnections\": {\n      \"type\": \"number\",\n      \"description\": \"Number of current client connections.\"\n    },\n    \"cursrvrconnections\": {\n      \"type\": \"number\",\n      \"description\": \"Number of current server connections.\"\n\
  \    },\n    \"establishedconn\": {\n      \"type\": \"number\",\n      \"description\": \"Number of connections in ESTABLISHED state.\"\n    },\n    \"tothits\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of virtual server hits.\"\n    },\n    \"hitsrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of hits per second.\"\n    },\n    \"totalrequests\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of requests received.\"\n    },\n    \"requestsrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of requests per second.\"\n    },\n    \"totalresponses\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of responses sent.\"\n    },\n    \"responsesrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of responses per second.\"\n    },\n    \"totalrequestbytes\": {\n      \"type\": \"number\",\n      \"description\": \"Total bytes of requests received.\"\n    },\n \
  \   \"totalresponsebytes\": {\n      \"type\": \"number\",\n      \"description\": \"Total bytes of responses sent.\"\n    },\n    \"totalpktsrecvd\": {\n      \"type\": \"number\",\n      \"description\": \"Total packets received.\"\n    },\n    \"totalpktssent\": {\n      \"type\": \"number\",\n      \"description\": \"Total packets sent.\"\n    },\n    \"totspillovers\": {\n      \"type\": \"number\",\n      \"description\": \"Total spillover events.\"\n    },\n    \"labelledconn\": {\n      \"type\": \"number\",\n      \"description\": \"Total labeled connections.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-cs-vserver-stats-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: CsVserverStats
---
