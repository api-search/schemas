---
description: Response for CheckIPAddressAvailability API service call.
layout: schema
name: IPAddressAvailabilityResult
properties_list:
- description: Private IP address availability.
  name: available
  type: boolean
- description: Contains other available private IP addresses if the asked for address is taken.
  name: availableIPAddresses
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-ip-address-availability-result-schema.json
slug: azure-networking-services-ip-address-availability-result
source_filename: azure-networking-services-ip-address-availability-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-ip-address-availability-result-schema.json\",\n  \"title\": \"IPAddressAvailabilityResult\",\n  \"description\": \"Response for CheckIPAddressAvailability API service call.\",\n  \"properties\": {\n    \"available\": {\n      \"description\": \"Private IP address availability.\",\n      \"type\": \"boolean\"\n    },\n    \"availableIPAddresses\": {\n      \"description\": \"Contains other available private IP addresses if the asked for address is taken.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-ip-address-availability-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: IPAddressAvailabilityResult
---
