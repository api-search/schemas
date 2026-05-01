---
description: Network interface on a source server
layout: schema
name: NetworkInterface
properties_list:
- description: MAC address
  name: macAddress
  type: string
- description: IP addresses
  name: ips
  type: array
- description: Whether this is the primary interface
  name: isPrimary
  type: boolean
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-network-interface-schema.json
slug: application-migration-service-network-interface
source_filename: application-migration-service-network-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\",\n  \"description\": \"Network interface on a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"macAddress\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address\"\n    },\n    \"ips\": {\n      \"type\": \"array\",\n      \"description\": \"IP addresses\"\n    },\n    \"isPrimary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary interface\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-network-interface-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: NetworkInterface
---
