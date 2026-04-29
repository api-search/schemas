---
description: Sales order item partner entity (A_SalesOrderItemPartner) representing a business partner in a specific function role at the item level.
layout: schema
name: SalesOrderItemPartner
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Sales order item number
  name: SalesOrderItem
  type: string
- description: Partner function code
  name: PartnerFunction
  type: string
- description: Customer number
  name: Customer
  type: string
- description: Supplier number
  name: Supplier
  type: string
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-item-partner-schema.json
slug: sap-s4hana-sales-order-sales-order-item-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderItemPartner\",\n  \"type\": \"object\",\n  \"description\": \"Sales order item partner entity (A_SalesOrderItemPartner) representing a business partner in a specific function role at the item level.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\"\n    },\n    \"SalesOrderItem\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order item number\"\n    },\n    \"PartnerFunction\": {\n      \"type\": \"string\",\n      \"description\": \"Partner function code\"\n    },\n    \"Customer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer number\"\n    },\n    \"Supplier\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-item-partner-schema.json
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
title: SalesOrderItemPartner
---
