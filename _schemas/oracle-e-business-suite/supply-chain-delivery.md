---
description: ''
layout: schema
name: Delivery
properties_list:
- description: Delivery identifier
  name: deliveryId
  type: integer
- description: Delivery name/number
  name: name
  type: string
- description: Delivery status code
  name: statusCode
  type: string
- description: Initial pickup date
  name: initialPickupDate
  type: string
- description: Ultimate dropoff date
  name: ultimateDropoffDate
  type: string
- description: Customer identifier
  name: customerId
  type: integer
- description: Ship-to location identifier
  name: shipToLocationId
  type: integer
- description: Carrier identifier
  name: carrierId
  type: integer
- description: Ship method code
  name: shipMethodCode
  type: string
- description: Waybill/tracking number
  name: waybill
  type: string
- description: Gross weight
  name: grossWeight
  type: number
- description: Weight unit of measure
  name: weightUomCode
  type: string
- description: Volume
  name: volume
  type: number
- description: Volume unit of measure
  name: volumeUomCode
  type: string
- description: ''
  name: organizationId
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-delivery-schema.json
slug: supply-chain-delivery
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Delivery\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveryId\": {\n      \"type\": \"integer\",\n      \"description\": \"Delivery identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery name/number\"\n    },\n    \"statusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery status code\"\n    },\n    \"initialPickupDate\": {\n      \"type\": \"string\",\n      \"description\": \"Initial pickup date\"\n    },\n    \"ultimateDropoffDate\": {\n      \"type\": \"string\",\n      \"description\": \"Ultimate dropoff date\"\n    },\n    \"customerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer identifier\"\n    },\n    \"shipToLocationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Ship-to location identifier\"\n    },\n    \"carrierId\": {\n      \"type\": \"integer\",\n     \
  \ \"description\": \"Carrier identifier\"\n    },\n    \"shipMethodCode\": {\n      \"type\": \"string\",\n      \"description\": \"Ship method code\"\n    },\n    \"waybill\": {\n      \"type\": \"string\",\n      \"description\": \"Waybill/tracking number\"\n    },\n    \"grossWeight\": {\n      \"type\": \"number\",\n      \"description\": \"Gross weight\"\n    },\n    \"weightUomCode\": {\n      \"type\": \"string\",\n      \"description\": \"Weight unit of measure\"\n    },\n    \"volume\": {\n      \"type\": \"number\",\n      \"description\": \"Volume\"\n    },\n    \"volumeUomCode\": {\n      \"type\": \"string\",\n      \"description\": \"Volume unit of measure\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-delivery-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Delivery
---
