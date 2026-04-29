---
description: Sales order header partner entity (A_SalesOrderHeaderPartner) representing a business partner in a specific partner function role at the header level.
layout: schema
name: SalesOrderHeaderPartner
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Partner function code (e.g., AG=Sold-to, WE=Ship-to, RE=Bill-to, RG=Payer)
  name: PartnerFunction
  type: string
- description: Customer number
  name: Customer
  type: string
- description: Supplier number
  name: Supplier
  type: string
- description: Personnel number
  name: Personnel
  type: string
- description: Contact person number
  name: ContactPerson
  type: string
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-header-partner-schema.json
slug: sap-s4hana-sales-order-sales-order-header-partner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderHeaderPartner\",\n  \"type\": \"object\",\n  \"description\": \"Sales order header partner entity (A_SalesOrderHeaderPartner) representing a business partner in a specific partner function role at the header level.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\"\n    },\n    \"PartnerFunction\": {\n      \"type\": \"string\",\n      \"description\": \"Partner function code (e.g., AG=Sold-to, WE=Ship-to, RE=Bill-to, RG=Payer)\"\n    },\n    \"Customer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer number\"\n    },\n    \"Supplier\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier number\"\n    },\n    \"Personnel\": {\n      \"type\": \"string\",\n      \"description\": \"Personnel number\"\n    },\n    \"ContactPerson\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Contact person number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-header-partner-schema.json
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
title: SalesOrderHeaderPartner
---
