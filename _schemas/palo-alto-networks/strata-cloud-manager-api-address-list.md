---
description: AddressList schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: AddressList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: offset
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-address-list-schema.json
slug: strata-cloud-manager-api-address-list
source_filename: strata-cloud-manager-api-address-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddressList\",\n  \"description\": \"AddressList schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An address object representing an IP address, subnet, range, or FQDN used in security policy rules.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\",\n            \"description\": \"Unique identifier assigned by the system.\",\n            \"readOnly\": true\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Unique name of the address object\
  \ within the folder scope.\"\n          },\n          \"folder\": {\n            \"type\": \"string\",\n            \"description\": \"Configuration folder containing this object.\",\n            \"readOnly\": true\n          },\n          \"snippet\": {\n            \"type\": \"string\",\n            \"readOnly\": true\n          },\n          \"ip_netmask\": {\n            \"type\": \"string\",\n            \"description\": \"IP address with CIDR netmask (e.g., 10.0.0.0/24).\"\n          },\n          \"ip_range\": {\n            \"type\": \"string\",\n            \"description\": \"IP address range (e.g., 10.0.0.1-10.0.0.254).\"\n          },\n          \"ip_wildcard\": {\n            \"type\": \"string\",\n            \"description\": \"IP wildcard mask notation.\"\n          },\n          \"fqdn\": {\n            \"type\": \"string\",\n            \"description\": \"Fully qualified domain name (e.g., www.example.com).\"\n          },\n          \"description\": {\n            \"type\"\
  : \"string\"\n          },\n          \"tag\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Tags assigned to this address object.\"\n          }\n        }\n      }\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AddressList
---
