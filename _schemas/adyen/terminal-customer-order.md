---
description: Customer order attached to a customer, recorded in the POI system. Allows the management of customer orders by the POI, for instance in a multi-channel or a click and collect sale transaction.
layout: schema
name: CustomerOrder
properties_list:
- description: Additional and optional identification of a customer order.
  name: CustomerOrderID
  type: string
- description: ''
  name: SaleReferenceID
  type: string
- description: ''
  name: OpenOrderState
  type: boolean
- description: Date time of the beginning of an operation.
  name: StartDate
  type: string
- description: Date time of the end of an operation.
  name: EndDate
  type: string
- description: ''
  name: ForecastedAmount
  type: number
- description: Total amount of all completed transactions of a customer order.
  name: CurrentAmount
  type: number
- description: Currency of a monetary amount.
  name: Currency
  type: string
- description: ''
  name: AccessedBy
  type: string
- description: Unqualified information.
  name: AdditionalInformation
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-customer-order-schema.json
slug: terminal-customer-order
source_filename: terminal-customer-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-customer-order-schema.json\",\n  \"title\": \"CustomerOrder\",\n  \"description\": \"Customer order attached to a customer, recorded in the POI system.  Allows the management of customer orders by the POI, for instance in a multi-channel or a click and collect sale transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerOrderID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Additional and optional identification of a customer order.\"\n    },\n    \"SaleReferenceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"OpenOrderState\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"StartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date time\
  \ of the beginning of an operation.\"\n    },\n    \"EndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date time of the end of an operation.\"\n    },\n    \"ForecastedAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"CurrentAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Total amount of all completed transactions of a customer order.\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n      \"description\": \"Currency of a monetary amount.\"\n    },\n    \"AccessedBy\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"AdditionalInformation\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Unqualified information.\"\n    }\n  },\n  \"required\": [\n    \"SaleReferenceID\",\n    \"StartDate\"\
  ,\n    \"ForecastedAmount\",\n    \"CurrentAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-customer-order-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CustomerOrder
---
