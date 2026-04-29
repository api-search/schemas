---
description: A paginated list of SAP HANA Cloud service instances in the subaccount.
layout: schema
name: ServiceInstanceList
properties_list:
- description: Total number of service instances matching the query criteria.
  name: num_items
  type: integer
- description: The list of service instances for the current page.
  name: items
  type: array
- description: Pagination token to retrieve the next page of results.
  name: token
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-service-instance-list-schema.json
slug: sap-hana-cloud-rest-service-instance-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceInstanceList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of SAP HANA Cloud service instances in the subaccount.\",\n  \"properties\": {\n    \"num_items\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of service instances matching the query criteria.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of service instances for the current page.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token to retrieve the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-service-instance-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: ServiceInstanceList
---
