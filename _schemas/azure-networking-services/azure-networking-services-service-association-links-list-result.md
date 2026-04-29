---
description: Response for ServiceAssociationLinks_List operation.
layout: schema
name: ServiceAssociationLinksListResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: The service association links in a subnet.
  name: value
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-service-association-links-list-result-schema.json
slug: azure-networking-services-service-association-links-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-association-links-list-result-schema.json\",\n  \"title\": \"ServiceAssociationLinksListResult\",\n  \"description\": \"Response for ServiceAssociationLinks_List operation.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The service association links in a subnet.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ServiceAssociationLink\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-association-links-list-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ServiceAssociationLinksListResult
---
