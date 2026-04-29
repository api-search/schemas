---
description: An address object representing an IP address, subnet, range, wildcard mask, or FQDN used in security policy rules.
layout: schema
name: Address
properties_list:
- description: Unique name of the address object.
  name: '@name'
  type: string
- description: IP address with CIDR netmask (e.g., 10.0.0.0/24).
  name: ip-netmask
  type: string
- description: IP address range (e.g., 10.0.0.1-10.0.0.254).
  name: ip-range
  type: string
- description: IP wildcard mask (e.g., 10.20.1.0/0.0.248.255).
  name: ip-wildcard
  type: string
- description: Fully qualified domain name (e.g., www.example.com).
  name: fqdn
  type: string
- description: Description of the address object.
  name: description
  type: string
- description: ''
  name: tag
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-address-schema.json
slug: pan-os-rest-api-address
source_filename: pan-os-rest-api-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"description\": \"An address object representing an IP address, subnet, range, wildcard mask, or FQDN used in security policy rules.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-address-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the address object.\"\n    },\n    \"ip-netmask\": {\n      \"type\": \"string\",\n      \"description\": \"IP address with CIDR netmask (e.g., 10.0.0.0/24).\"\n    },\n    \"ip-range\": {\n      \"type\": \"string\",\n      \"description\": \"IP address range (e.g., 10.0.0.1-10.0.0.254).\"\n    },\n    \"ip-wildcard\": {\n      \"type\": \"string\",\n      \"description\": \"IP wildcard mask (e.g., 10.20.1.0/0.0.248.255).\"\n    },\n    \"fqdn\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Fully qualified domain name (e.g., www.example.com).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the address object.\"\n    },\n    \"tag\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Tags assigned to this address object.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-address-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Address
---
