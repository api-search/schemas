---
description: Sales order header text entity (A_SalesOrderText) for long texts associated with the sales order header.
layout: schema
name: SalesOrderText
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Language key (ISO 639-1)
  name: Language
  type: string
- description: Text ID (e.g., 0001 for header note)
  name: LongTextID
  type: string
- description: Text content
  name: LongText
  type: string
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-text-schema.json
slug: sap-s4hana-sales-order-sales-order-text
source_filename: sap-s4hana-sales-order-sales-order-text-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderText\",\n  \"type\": \"object\",\n  \"description\": \"Sales order header text entity (A_SalesOrderText) for long texts associated with the sales order header.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\"\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"description\": \"Language key (ISO 639-1)\"\n    },\n    \"LongTextID\": {\n      \"type\": \"string\",\n      \"description\": \"Text ID (e.g., 0001 for header note)\"\n    },\n    \"LongText\": {\n      \"type\": \"string\",\n      \"description\": \"Text content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-text-schema.json
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
title: SalesOrderText
---
