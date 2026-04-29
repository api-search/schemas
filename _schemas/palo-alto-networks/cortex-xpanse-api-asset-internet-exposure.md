---
description: Summary of an internet-exposed asset discovered by Xpanse.
layout: schema
name: AssetInternetExposure
properties_list:
- description: List of ASM identifiers for this asset.
  name: asm_id_list
  type: array
- description: Asset hostname, IP address, or identifier.
  name: asset_name
  type: string
- description: ''
  name: asset_type
  type: string
- description: IP addresses associated with this asset.
  name: ip_address
  type: array
- description: Domain names associated with this asset.
  name: domain
  type: array
- description: ''
  name: ipv6_address
  type: array
- description: Cloud provider resource identifier.
  name: cloud_id
  type: string
- description: ''
  name: cloud_provider
  type: string
- description: ''
  name: externally_detected_providers
  type: array
- description: Business units associated with this asset.
  name: business_units
  type: array
- description: ''
  name: tags
  type: array
- description: Asset first discovery timestamp as Unix epoch milliseconds.
  name: created
  type: integer
- description: Most recent observation timestamp as Unix epoch milliseconds.
  name: last_observed
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-asset-internet-exposure-schema.json
slug: cortex-xpanse-api-asset-internet-exposure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetInternetExposure\",\n  \"description\": \"Summary of an internet-exposed asset discovered by Xpanse.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-asset-internet-exposure-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asm_id_list\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of ASM identifiers for this asset.\"\n    },\n    \"asset_name\": {\n      \"type\": \"string\",\n      \"description\": \"Asset hostname, IP address, or identifier.\"\n    },\n    \"asset_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CERTIFICATE\",\n        \"CLOUD_COMPUTE_INSTANCE\",\n        \"CLOUD_LOAD_BALANCER\",\n        \"CLOUD_OBJECT_STORAGE\",\n        \"DOMAIN\",\n        \"NETWORKING_DEVICE\",\n     \
  \   \"ON_PREM_SERVER\",\n        \"UNMANAGED_NETWORK_DEVICE\"\n      ]\n    },\n    \"ip_address\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IP addresses associated with this asset.\"\n    },\n    \"domain\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Domain names associated with this asset.\"\n    },\n    \"ipv6_address\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"cloud_id\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider resource identifier.\"\n    },\n    \"cloud_provider\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AWS\",\n        \"Azure\",\n        \"GCP\",\n        \"OTHER\"\n      ]\n    },\n    \"externally_detected_providers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n \
  \   \"business_units\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Business units associated with this asset.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Asset first discovery timestamp as Unix epoch milliseconds.\"\n    },\n    \"last_observed\": {\n      \"type\": \"integer\",\n      \"description\": \"Most recent observation timestamp as Unix epoch milliseconds.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-asset-internet-exposure-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AssetInternetExposure
---
