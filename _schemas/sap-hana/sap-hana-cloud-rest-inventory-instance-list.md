---
description: A paginated list of SAP HANA Cloud instances from the inventory service.
layout: schema
name: InventoryInstanceList
properties_list:
- description: Total number of instances matching the query criteria.
  name: totalCount
  type: integer
- description: The list of inventory instances for the current page.
  name: items
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-inventory-instance-list-schema.json
slug: sap-hana-cloud-rest-inventory-instance-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryInstanceList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of SAP HANA Cloud instances from the inventory service.\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of instances matching the query criteria.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of inventory instances for the current page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-inventory-instance-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: InventoryInstanceList
---
