---
description: Sales order item pricing element entity (A_SalesOrderItemPrcgElmnt) representing a pricing condition at the item level.
layout: schema
name: SalesOrderItemPrcgElmnt
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Sales order item number
  name: SalesOrderItem
  type: string
- description: Step number in the pricing procedure
  name: PricingProcedureStep
  type: string
- description: Counter for condition within a step
  name: PricingProcedureCounter
  type: string
- description: Condition type
  name: ConditionType
  type: string
- description: Condition rate
  name: ConditionRateValue
  type: string
- description: Condition currency
  name: ConditionCurrency
  type: string
- description: Condition quantity
  name: ConditionQuantity
  type: string
- description: Condition quantity unit
  name: ConditionQuantityUnit
  type: string
- description: Condition value
  name: ConditionAmount
  type: string
- description: Document currency
  name: TransactionCurrency
  type: string
- description: Condition category
  name: ConditionCategory
  type: string
- description: Statistical condition
  name: ConditionIsForStatistics
  type: boolean
- description: Origin of the condition
  name: ConditionOrigin
  type: string
- description: Group condition indicator
  name: IsGroupCondition
  type: string
- description: Condition control
  name: ConditionControl
  type: string
- description: Reason for inactivity
  name: ConditionInactiveReason
  type: string
- description: Condition class
  name: ConditionClass
  type: string
- description: Manually changed indicator
  name: ConditionIsManuallyChanged
  type: boolean
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-item-prcg-elmnt-schema.json
slug: sap-s4hana-sales-order-sales-order-item-prcg-elmnt
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderItemPrcgElmnt\",\n  \"type\": \"object\",\n  \"description\": \"Sales order item pricing element entity (A_SalesOrderItemPrcgElmnt) representing a pricing condition at the item level.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\"\n    },\n    \"SalesOrderItem\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order item number\"\n    },\n    \"PricingProcedureStep\": {\n      \"type\": \"string\",\n      \"description\": \"Step number in the pricing procedure\"\n    },\n    \"PricingProcedureCounter\": {\n      \"type\": \"string\",\n      \"description\": \"Counter for condition within a step\"\n    },\n    \"ConditionType\": {\n      \"type\": \"string\",\n      \"description\": \"Condition type\"\n    },\n    \"ConditionRateValue\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Condition rate\"\n    },\n    \"ConditionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Condition currency\"\n    },\n    \"ConditionQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"Condition quantity\"\n    },\n    \"ConditionQuantityUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Condition quantity unit\"\n    },\n    \"ConditionAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Condition value\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Document currency\"\n    },\n    \"ConditionCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Condition category\"\n    },\n    \"ConditionIsForStatistics\": {\n      \"type\": \"boolean\",\n      \"description\": \"Statistical condition\"\n    },\n    \"ConditionOrigin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin of the condition\"\n    },\n    \"IsGroupCondition\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Group condition indicator\"\n    },\n    \"ConditionControl\": {\n      \"type\": \"string\",\n      \"description\": \"Condition control\"\n    },\n    \"ConditionInactiveReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for inactivity\"\n    },\n    \"ConditionClass\": {\n      \"type\": \"string\",\n      \"description\": \"Condition class\"\n    },\n    \"ConditionIsManuallyChanged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Manually changed indicator\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-item-prcg-elmnt-schema.json
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
title: SalesOrderItemPrcgElmnt
---
