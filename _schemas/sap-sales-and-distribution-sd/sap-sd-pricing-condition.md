---
description: Schema for SAP S/4HANA Sales Pricing Condition Record entity (A_SlsPrcgConditionRecord) from the API_SLSPRCGCONDITIONRECORD_SRV OData service. Represents a pricing condition record used to determine prices, discounts, and surcharges in sales documents.
layout: schema
name: SAP Pricing Condition Record
properties_list:
- description: Condition record number
  name: ConditionRecord
  type: string
- description: Sequential number of the condition
  name: ConditionSequentialNumber
  type: string
- description: Condition table
  name: ConditionTable
  type: string
- description: Condition type (e.g., PR00=Price, K004=Material Discount, K005=Customer/Material Discount, K007=Customer Discount)
  name: ConditionType
  type: string
- description: Validity start date
  name: ConditionValidityStartDate
  type: string
- description: Validity end date
  name: ConditionValidityEndDate
  type: string
- description: Rate (condition amount or percentage)
  name: ConditionRateValue
  type: string
- description: Condition currency or percentage
  name: ConditionRateValueUnit
  type: string
- description: Condition pricing unit
  name: ConditionQuantity
  type: string
- description: Condition unit
  name: ConditionQuantityUnit
  type: string
- description: Calculation type for the condition
  name: ConditionCalculationType
  type: string
- description: Deletion indicator
  name: ConditionIsDeleted
  type: boolean
- description: Sales organization
  name: SalesOrganization
  type: string
- description: Distribution channel
  name: DistributionChannel
  type: string
- description: Material number
  name: Material
  type: string
- description: Customer number
  name: Customer
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-pricing-condition-schema.json
slug: sap-sd-pricing-condition
source_filename: sap-sd-pricing-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-pricing-condition\",\n  \"title\": \"SAP Pricing Condition Record\",\n  \"description\": \"Schema for SAP S/4HANA Sales Pricing Condition Record entity (A_SlsPrcgConditionRecord) from the API_SLSPRCGCONDITIONRECORD_SRV OData service. Represents a pricing condition record used to determine prices, discounts, and surcharges in sales documents.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConditionRecord\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Condition record number\"\n    },\n    \"ConditionSequentialNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Sequential number of the condition\"\n    },\n    \"ConditionTable\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Condition table\"\n    },\n    \"ConditionType\": {\n      \"type\"\
  : \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Condition type (e.g., PR00=Price, K004=Material Discount, K005=Customer/Material Discount, K007=Customer Discount)\"\n    },\n    \"ConditionValidityStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Validity start date\"\n    },\n    \"ConditionValidityEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Validity end date\"\n    },\n    \"ConditionRateValue\": {\n      \"type\": \"string\",\n      \"description\": \"Rate (condition amount or percentage)\"\n    },\n    \"ConditionRateValueUnit\": {\n      \"type\": \"string\",\n      \"maxLength\": 5,\n      \"description\": \"Condition currency or percentage\"\n    },\n    \"ConditionQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"Condition pricing unit\"\n    },\n    \"ConditionQuantityUnit\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"\
  description\": \"Condition unit\"\n    },\n    \"ConditionCalculationType\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Calculation type for the condition\"\n    },\n    \"ConditionIsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deletion indicator\"\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales organization\"\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Distribution channel\"\n    },\n    \"Material\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"Material number\"\n    },\n    \"Customer\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Customer number\"\n    }\n  },\n  \"required\": [\"ConditionRecord\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-pricing-condition-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Pricing Condition Record
---
