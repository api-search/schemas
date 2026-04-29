---
description: Request body for creating or updating an address object.
layout: schema
name: AddressRequest
properties_list:
- description: ''
  name: name
  type: string
- description: IP address with CIDR netmask (e.g., 10.0.0.0/24).
  name: ip_netmask
  type: string
- description: IP address range (e.g., 10.0.0.1-10.0.0.254).
  name: ip_range
  type: string
- description: IP wildcard mask notation.
  name: ip_wildcard
  type: string
- description: Fully qualified domain name.
  name: fqdn
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-address-request-schema.json
slug: strata-cloud-manager-api-address-request
source_filename: strata-cloud-manager-api-address-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddressRequest\",\n  \"description\": \"Request body for creating or updating an address object.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"ip_netmask\": {\n      \"type\": \"string\",\n      \"description\": \"IP address with CIDR netmask (e.g., 10.0.0.0/24).\"\n    },\n    \"ip_range\": {\n      \"type\": \"string\",\n      \"description\": \"IP address range (e.g., 10.0.0.1-10.0.0.254).\"\n    },\n    \"ip_wildcard\": {\n      \"type\": \"string\",\n      \"description\": \"IP wildcard mask notation.\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified domain name.\"\n    },\n    \"description\": {\n      \"type\": \"\
  string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AddressRequest
---
