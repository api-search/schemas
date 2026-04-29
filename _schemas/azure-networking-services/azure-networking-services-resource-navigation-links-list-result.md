---
description: Response for ResourceNavigationLinks_List operation.
layout: schema
name: ResourceNavigationLinksListResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: The resource navigation links in a subnet.
  name: value
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-resource-navigation-links-list-result-schema.json
slug: azure-networking-services-resource-navigation-links-list-result
source_filename: azure-networking-services-resource-navigation-links-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-resource-navigation-links-list-result-schema.json\",\n  \"title\": \"ResourceNavigationLinksListResult\",\n  \"description\": \"Response for ResourceNavigationLinks_List operation.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The resource navigation links in a subnet.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ResourceNavigationLink\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-resource-navigation-links-list-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ResourceNavigationLinksListResult
---
