---
description: An internet-exposed network service discovered on an asset.
layout: schema
name: ExposedService
properties_list:
- description: ''
  name: service_id
  type: string
- description: Service name or protocol (e.g., HTTPS, SSH, RDP).
  name: service_name
  type: string
- description: ''
  name: service_type
  type: string
- description: ''
  name: ip_address
  type: array
- description: ''
  name: domain
  type: array
- description: TCP/UDP port number.
  name: port
  type: integer
- description: ''
  name: protocol
  type: string
- description: Cloud or hosting providers detected for this service.
  name: provider
  type: array
- description: ''
  name: business_units
  type: array
- description: Service first discovery timestamp as Unix epoch milliseconds.
  name: created
  type: integer
- description: ''
  name: last_observed
  type: integer
- description: ''
  name: is_active
  type: string
- description: ''
  name: discovery_type
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-exposed-service-schema.json
slug: cortex-xpanse-api-exposed-service
source_filename: cortex-xpanse-api-exposed-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExposedService\",\n  \"description\": \"An internet-exposed network service discovered on an asset.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-exposed-service-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_id\": {\n      \"type\": \"string\"\n    },\n    \"service_name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name or protocol (e.g., HTTPS, SSH, RDP).\"\n    },\n    \"service_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"APPLICATION_SERVER\",\n        \"CLOUD_STORAGE\",\n        \"DATABASE\",\n        \"NETWORKING\",\n        \"REMOTE_DESKTOP\",\n        \"UNCLASSIFIED\",\n        \"WEB\"\n      ]\n    },\n    \"ip_address\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"\
  domain\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"TCP/UDP port number.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TCP\",\n        \"UDP\"\n      ]\n    },\n    \"provider\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Cloud or hosting providers detected for this service.\"\n    },\n    \"business_units\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Service first discovery timestamp as Unix epoch milliseconds.\"\n    },\n    \"last_observed\": {\n      \"type\": \"integer\"\n    },\n    \"is_active\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Inactive\",\n        \"Unconfirmed\"\
  \n      ]\n    },\n    \"discovery_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ColocatedOnIp\",\n        \"DirectlyDiscovered\",\n        \"CSP\",\n        \"CertificateAssociation\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-exposed-service-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ExposedService
---
