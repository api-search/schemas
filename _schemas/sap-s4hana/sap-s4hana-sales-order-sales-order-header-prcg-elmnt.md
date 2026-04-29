---
description: Sales order header pricing element entity (A_SalesOrderHeaderPrcgElmnt) representing a pricing condition at the header level, such as overall discounts, surcharges, or freight.
layout: schema
name: SalesOrderHeaderPrcgElmnt
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Step number in the pricing procedure
  name: PricingProcedureStep
  type: string
- description: Counter for condition within a step
  name: PricingProcedureCounter
  type: string
- description: Condition type (e.g., PR00 for price, K004 for discount, MWST for tax)
  name: ConditionType
  type: string
- description: Condition rate or amount per pricing unit
  name: ConditionRateValue
  type: string
- description: Currency for the condition
  name: ConditionCurrency
  type: string
- description: Condition pricing quantity
  name: ConditionQuantity
  type: string
- description: Condition quantity unit
  name: ConditionQuantityUnit
  type: string
- description: Condition category
  name: ConditionCategory
  type: string
- description: Statistical condition indicator
  name: ConditionIsForStatistics
  type: boolean
- description: Scale type
  name: PricingScaleType
  type: string
- description: Accrual indicator
  name: IsRelevantForAccrual
  type: boolean
- description: Origin of the condition
  name: ConditionOrigin
  type: string
- description: Group condition indicator
  name: IsGroupCondition
  type: string
- description: Condition value (total amount for the condition)
  name: ConditionAmount
  type: string
- description: Document currency
  name: TransactionCurrency
  type: string
- description: Condition control
  name: ConditionControl
  type: string
- description: Reason the condition is inactive
  name: ConditionInactiveReason
  type: string
- description: Condition class (A=discount, B=surcharge)
  name: ConditionClass
  type: string
- description: Procedure counter for header conditions
  name: PrcgProcedureCounterForHeader
  type: string
- description: Factor for condition basis value
  name: FactorForConditionBasisValue
  type: string
- description: Structure condition
  name: StructureCondition
  type: string
- description: Period factor for condition basis value
  name: PeriodFactorForCndnBasisValue
  type: string
- description: Scale basis indicator
  name: PricingScaleBasis
  type: string
- description: Scale basis value
  name: ConditionScaleBasisValue
  type: string
- description: Condition scale basis unit
  name: ConditionScaleBasisUnit
  type: string
- description: Scale basis currency
  name: ConditionScaleBasisCurrency
  type: string
- description: Relevant for intercompany billing
  name: CndnIsRelevantForIntcoBilling
  type: boolean
- description: Indicator that the condition was manually changed
  name: ConditionIsManuallyChanged
  type: boolean
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-header-prcg-elmnt-schema.json
slug: sap-s4hana-sales-order-sales-order-header-prcg-elmnt
source_filename: sap-s4hana-sales-order-sales-order-header-prcg-elmnt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderHeaderPrcgElmnt\",\n  \"type\": \"object\",\n  \"description\": \"Sales order header pricing element entity (A_SalesOrderHeaderPrcgElmnt) representing a pricing condition at the header level, such as overall discounts, surcharges, or freight.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\"\n    },\n    \"PricingProcedureStep\": {\n      \"type\": \"string\",\n      \"description\": \"Step number in the pricing procedure\"\n    },\n    \"PricingProcedureCounter\": {\n      \"type\": \"string\",\n      \"description\": \"Counter for condition within a step\"\n    },\n    \"ConditionType\": {\n      \"type\": \"string\",\n      \"description\": \"Condition type (e.g., PR00 for price, K004 for discount, MWST for tax)\"\n    },\n    \"ConditionRateValue\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Condition rate or amount per pricing unit\"\n    },\n    \"ConditionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency for the condition\"\n    },\n    \"ConditionQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"Condition pricing quantity\"\n    },\n    \"ConditionQuantityUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Condition quantity unit\"\n    },\n    \"ConditionCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Condition category\"\n    },\n    \"ConditionIsForStatistics\": {\n      \"type\": \"boolean\",\n      \"description\": \"Statistical condition indicator\"\n    },\n    \"PricingScaleType\": {\n      \"type\": \"string\",\n      \"description\": \"Scale type\"\n    },\n    \"IsRelevantForAccrual\": {\n      \"type\": \"boolean\",\n      \"description\": \"Accrual indicator\"\n    },\n    \"ConditionOrigin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin of the condition\"\n\
  \    },\n    \"IsGroupCondition\": {\n      \"type\": \"string\",\n      \"description\": \"Group condition indicator\"\n    },\n    \"ConditionAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Condition value (total amount for the condition)\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Document currency\"\n    },\n    \"ConditionControl\": {\n      \"type\": \"string\",\n      \"description\": \"Condition control\"\n    },\n    \"ConditionInactiveReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason the condition is inactive\"\n    },\n    \"ConditionClass\": {\n      \"type\": \"string\",\n      \"description\": \"Condition class (A=discount, B=surcharge)\"\n    },\n    \"PrcgProcedureCounterForHeader\": {\n      \"type\": \"string\",\n      \"description\": \"Procedure counter for header conditions\"\n    },\n    \"FactorForConditionBasisValue\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Factor for condition basis value\"\n    },\n    \"StructureCondition\": {\n      \"type\": \"string\",\n      \"description\": \"Structure condition\"\n    },\n    \"PeriodFactorForCndnBasisValue\": {\n      \"type\": \"string\",\n      \"description\": \"Period factor for condition basis value\"\n    },\n    \"PricingScaleBasis\": {\n      \"type\": \"string\",\n      \"description\": \"Scale basis indicator\"\n    },\n    \"ConditionScaleBasisValue\": {\n      \"type\": \"string\",\n      \"description\": \"Scale basis value\"\n    },\n    \"ConditionScaleBasisUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Condition scale basis unit\"\n    },\n    \"ConditionScaleBasisCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Scale basis currency\"\n    },\n    \"CndnIsRelevantForIntcoBilling\": {\n      \"type\": \"boolean\",\n      \"description\": \"Relevant for intercompany billing\"\n    },\n    \"ConditionIsManuallyChanged\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Indicator that the condition was manually changed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-header-prcg-elmnt-schema.json
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
title: SalesOrderHeaderPrcgElmnt
---
