---
description: A content switching virtual server that directs client requests to different load balancing virtual servers based on content switching policies evaluating request attributes such as URL, HTTP header, or source IP address.
layout: schema
name: CsVserver
properties_list:
- description: Name for the content switching virtual server. Must be unique and begin with a letter, number, or underscore. Maximum 127 characters.
  name: name
  type: string
- description: Traffic domain identifier. Range 0-4094.
  name: td
  type: integer
- description: Protocol of the service running on the virtual server.
  name: servicetype
  type: string
- description: IPv4 or IPv6 address of the content switching virtual server.
  name: ipv46
  type: string
- description: Port number on which the content switching virtual server listens.
  name: port
  type: integer
- description: Name of the IP set to bind to the virtual server.
  name: ipset
  type: string
- description: Number of consecutive IP addresses for the virtual server. Range 2-254.
  name: range
  type: integer
- description: IP address pattern for matching incoming requests.
  name: ippattern
  type: string
- description: IP mask applied with ippattern to form an address range.
  name: ipmask
  type: string
- description: Whether the virtual server checks the backend server state for updates.
  name: stateupdate
  type: string
- description: Type of precedence for content switching policies. RULE means policies are evaluated in priority order. URL means URL-based switching takes precedence.
  name: precedence
  type: string
- description: Whether URL-based content switching is case sensitive.
  name: casesensitive
  type: string
- description: Spillover method for the content switching virtual server.
  name: somethod
  type: string
- description: Whether to maintain persistence during spillover.
  name: sopersistence
  type: string
- description: Persistence timeout in minutes during spillover. Range 2-1440.
  name: sopersistencetimeout
  type: integer
- description: Threshold value for the spillover method.
  name: sothreshold
  type: integer
- description: URL to redirect requests to when the virtual server is DOWN.
  name: redirecturl
  type: string
- description: Client idle timeout in seconds. Range 0-31536000.
  name: clttimeout
  type: integer
- description: Flush all active transactions when the virtual server goes DOWN.
  name: downstateflush
  type: string
- description: Insert the virtual server VIP address and port into the HTTP header of the request.
  name: insertvserveripport
  type: string
- description: Name of the HTTP header in which the VIP is inserted.
  name: vipheader
  type: string
- description: Continue to direct traffic to the virtual server even when DOWN in HA mode.
  name: disableprimaryondown
  type: string
- description: Whether authentication is enabled for the virtual server.
  name: authentication
  type: string
- description: FQDN of the authentication virtual server.
  name: authenticationhost
  type: string
- description: Whether HTTP 401-based authentication is enabled.
  name: authn401
  type: string
- description: Name of the authentication virtual server.
  name: authnvsname
  type: string
- description: Whether push functionality is enabled.
  name: push
  type: string
- description: Expression for extracting a label from the request.
  name: pushlabel
  type: string
- description: Allow multiple clients to connect to the push vserver.
  name: pushmulticlients
  type: string
- description: Description or comments about the content switching virtual server.
  name: comment
  type: string
- description: Whether Layer 2 connectivity is enabled between the client and server.
  name: l2conn
  type: string
- description: How the appliance responds to ICMP ping requests for the VIP.
  name: icmpvsrresponse
  type: string
- description: Route health injection state for the virtual server.
  name: rhistate
  type: string
- description: Whether to log AppFlow records for the virtual server.
  name: appflowlog
  type: string
- description: Administrative state of the virtual server.
  name: state
  type: string
- description: Name of the default load balancing virtual server bound to this content switching virtual server. Requests that do not match any policy are sent here.
  name: lbvserver
  type: string
- description: Name of the target load balancing virtual server to which content is switched.
  name: targetlbvserver
  type: string
- description: Cache type for integrated caching.
  name: cachetype
  type: string
- description: Type of cache redirect for the virtual server.
  name: redirect
  type: string
- description: Current operational state of the virtual server.
  name: curstate
  type: string
- description: Current status of the virtual server. 1 indicates UP.
  name: status
  type: integer
- description: Time when the virtual server state last changed.
  name: statechangetimesec
  type: string
- description: Number of ticks since the last state change.
  name: tickssincelaststatechange
  type: integer
- description: Virtual server type (e.g., content-based or IP-address based).
  name: type
  type: string
- description: Node group name to which the virtual server is bound.
  name: ngname
  type: string
- description: The value of the IP address, based on the virtual server type.
  name: value
  type: string
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-cs-vserver-schema.json
slug: citrix-netscaler-nitro-cs-vserver
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CsVserver\",\n  \"type\": \"object\",\n  \"description\": \"A content switching virtual server that directs client requests to different load balancing virtual servers based on content switching policies evaluating request attributes such as URL, HTTP header, or source IP address.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the content switching virtual server. Must be unique and begin with a letter, number, or underscore. Maximum 127 characters.\"\n    },\n    \"td\": {\n      \"type\": \"integer\",\n      \"description\": \"Traffic domain identifier. Range 0-4094.\"\n    },\n    \"servicetype\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol of the service running on the virtual server.\"\n    },\n    \"ipv46\": {\n      \"type\": \"string\",\n      \"description\": \"IPv4 or IPv6 address of the content switching\
  \ virtual server.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number on which the content switching virtual server listens.\"\n    },\n    \"ipset\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the IP set to bind to the virtual server.\"\n    },\n    \"range\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consecutive IP addresses for the virtual server. Range 2-254.\"\n    },\n    \"ippattern\": {\n      \"type\": \"string\",\n      \"description\": \"IP address pattern for matching incoming requests.\"\n    },\n    \"ipmask\": {\n      \"type\": \"string\",\n      \"description\": \"IP mask applied with ippattern to form an address range.\"\n    },\n    \"stateupdate\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the virtual server checks the backend server state for updates.\"\n    },\n    \"precedence\": {\n      \"type\": \"string\",\n      \"description\": \"Type of precedence\
  \ for content switching policies. RULE means policies are evaluated in priority order. URL means URL-based switching takes precedence.\"\n    },\n    \"casesensitive\": {\n      \"type\": \"string\",\n      \"description\": \"Whether URL-based content switching is case sensitive.\"\n    },\n    \"somethod\": {\n      \"type\": \"string\",\n      \"description\": \"Spillover method for the content switching virtual server.\"\n    },\n    \"sopersistence\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to maintain persistence during spillover.\"\n    },\n    \"sopersistencetimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Persistence timeout in minutes during spillover. Range 2-1440.\"\n    },\n    \"sothreshold\": {\n      \"type\": \"integer\",\n      \"description\": \"Threshold value for the spillover method.\"\n    },\n    \"redirecturl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to redirect requests to when the virtual server\
  \ is DOWN.\"\n    },\n    \"clttimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Client idle timeout in seconds. Range 0-31536000.\"\n    },\n    \"downstateflush\": {\n      \"type\": \"string\",\n      \"description\": \"Flush all active transactions when the virtual server goes DOWN.\"\n    },\n    \"insertvserveripport\": {\n      \"type\": \"string\",\n      \"description\": \"Insert the virtual server VIP address and port into the HTTP header of the request.\"\n    },\n    \"vipheader\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the HTTP header in which the VIP is inserted.\"\n    },\n    \"disableprimaryondown\": {\n      \"type\": \"string\",\n      \"description\": \"Continue to direct traffic to the virtual server even when DOWN in HA mode.\"\n    },\n    \"authentication\": {\n      \"type\": \"string\",\n      \"description\": \"Whether authentication is enabled for the virtual server.\"\n    },\n    \"authenticationhost\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"FQDN of the authentication virtual server.\"\n    },\n    \"authn401\": {\n      \"type\": \"string\",\n      \"description\": \"Whether HTTP 401-based authentication is enabled.\"\n    },\n    \"authnvsname\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the authentication virtual server.\"\n    },\n    \"push\": {\n      \"type\": \"string\",\n      \"description\": \"Whether push functionality is enabled.\"\n    },\n    \"pushlabel\": {\n      \"type\": \"string\",\n      \"description\": \"Expression for extracting a label from the request.\"\n    },\n    \"pushmulticlients\": {\n      \"type\": \"string\",\n      \"description\": \"Allow multiple clients to connect to the push vserver.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Description or comments about the content switching virtual server.\"\n    },\n    \"l2conn\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Whether Layer 2 connectivity is enabled between the client and server.\"\n    },\n    \"icmpvsrresponse\": {\n      \"type\": \"string\",\n      \"description\": \"How the appliance responds to ICMP ping requests for the VIP.\"\n    },\n    \"rhistate\": {\n      \"type\": \"string\",\n      \"description\": \"Route health injection state for the virtual server.\"\n    },\n    \"appflowlog\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to log AppFlow records for the virtual server.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative state of the virtual server.\"\n    },\n    \"lbvserver\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the default load balancing virtual server bound to this content switching virtual server. Requests that do not match any policy are sent here.\"\n    },\n    \"targetlbvserver\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target load balancing\
  \ virtual server to which content is switched.\"\n    },\n    \"cachetype\": {\n      \"type\": \"string\",\n      \"description\": \"Cache type for integrated caching.\"\n    },\n    \"redirect\": {\n      \"type\": \"string\",\n      \"description\": \"Type of cache redirect for the virtual server.\"\n    },\n    \"curstate\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state of the virtual server.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Current status of the virtual server. 1 indicates UP.\"\n    },\n    \"statechangetimesec\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the virtual server state last changed.\"\n    },\n    \"tickssincelaststatechange\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of ticks since the last state change.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual server type (e.g., content-based or IP-address\
  \ based).\"\n    },\n    \"ngname\": {\n      \"type\": \"string\",\n      \"description\": \"Node group name to which the virtual server is bound.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the IP address, based on the virtual server type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-cs-vserver-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: CsVserver
---
