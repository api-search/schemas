---
description: A route in the Bloomberg Execution Management System (EMSX) representing the assignment of an order (or portion thereof) to a specific broker for execution. Routes contain broker details, execution strategy, pricing instructions, and fill status.
layout: schema
name: Bloomberg EMSX Route
properties_list:
- description: EMSX route identifier, unique within the blotter
  name: routeId
  type: integer
- description: Parent order sequence number linking this route to its order
  name: orderSequenceNumber
  type: integer
- description: Bloomberg security ticker symbol
  name: ticker
  type: string
- description: Route side, inherited from the parent order
  name: side
  type: string
- description: Quantity assigned to this route
  name: amount
  type: number
- description: Quantity filled on this route
  name: filledAmount
  type: number
- description: Volume-weighted average fill price on this route
  name: averagePrice
  type: number
- description: Remaining unfilled quantity on this route
  name: remainingAmount
  type: number
- description: Bloomberg broker code identifying the executing broker
  name: broker
  type: string
- description: Full name of the executing broker
  name: brokerName
  type: string
- description: Execution strategy name (e.g., VWAP, TWAP, DMA, Iceberg)
  name: strategy
  type: string
- description: Strategy-specific configurable parameters
  name: strategyParameters
  type: object
- description: Current lifecycle status of the route
  name: status
  type: string
- description: Limit price for the route
  name: limitPrice
  type: number
- description: Order type on the route
  name: orderType
  type: string
- description: Time in force on the route
  name: timeInForce
  type: string
- description: Trading account identifier
  name: account
  type: string
- description: Destination exchange or marketplace
  name: exchange
  type: string
- description: Rejection or cancellation reason code from the broker
  name: reasonCode
  type: string
- description: Human-readable reason for rejection or cancellation
  name: reasonDescription
  type: string
- description: ISO 8601 timestamp when the route was created
  name: createdTime
  type: string
- description: ISO 8601 timestamp when the route was last modified
  name: lastModifiedTime
  type: string
- description: ISO 8601 timestamp of the most recent fill on this route
  name: lastFillTime
  type: string
- description: Custom user-defined fields
  name: customFields
  type: object
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
schema_file: json-schema/bloomberg-emsx-route-schema.json
slug: bloomberg-emsx-route
source_filename: bloomberg-emsx-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.bloomberg.com/schemas/emsx/route.json\",\n  \"title\": \"Bloomberg EMSX Route\",\n  \"description\": \"A route in the Bloomberg Execution Management System (EMSX) representing the assignment of an order (or portion thereof) to a specific broker for execution. Routes contain broker details, execution strategy, pricing instructions, and fill status.\",\n  \"type\": \"object\",\n  \"required\": [\"orderSequenceNumber\", \"broker\", \"amount\"],\n  \"properties\": {\n    \"routeId\": {\n      \"type\": \"integer\",\n      \"description\": \"EMSX route identifier, unique within the blotter\"\n    },\n    \"orderSequenceNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent order sequence number linking this route to its order\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security ticker symbol\"\n    },\n    \"side\": {\n\
  \      \"type\": \"string\",\n      \"enum\": [\"BUY\", \"SELL\", \"SHORT\", \"COVER\"],\n      \"description\": \"Route side, inherited from the parent order\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"description\": \"Quantity assigned to this route\"\n    },\n    \"filledAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Quantity filled on this route\"\n    },\n    \"averagePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Volume-weighted average fill price on this route\"\n    },\n    \"remainingAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Remaining unfilled quantity on this route\"\n    },\n    \"broker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg broker code identifying the executing broker\"\n    },\n    \"brokerName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the executing broker\"\
  \n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"description\": \"Execution strategy name (e.g., VWAP, TWAP, DMA, Iceberg)\"\n    },\n    \"strategyParameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Strategy-specific configurable parameters\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"NEW\", \"WORKING\", \"PARTIALLY_FILLED\", \"FILLED\", \"CANCELLED\", \"REJECTED\"],\n      \"description\": \"Current lifecycle status of the route\"\n    },\n    \"limitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Limit price for the route\"\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"enum\": [\"MKT\", \"LMT\", \"STP\", \"STP_LMT\", \"MOC\", \"LOC\", \"VWAP\", \"TWAP\"],\n      \"description\": \"Order type on the route\"\n    },\n    \"timeInForce\": {\n      \"type\": \"string\",\n      \"enum\": [\"DAY\", \"GTC\", \"IOC\", \"FOK\", \"GTD\", \"OPG\"\
  , \"CLO\"],\n      \"description\": \"Time in force on the route\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Trading account identifier\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Destination exchange or marketplace\"\n    },\n    \"reasonCode\": {\n      \"type\": \"string\",\n      \"description\": \"Rejection or cancellation reason code from the broker\"\n    },\n    \"reasonDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable reason for rejection or cancellation\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the route was created\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the route was last modified\"\n    },\n    \"lastFillTime\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the most recent fill on this route\"\n    },\n    \"customFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom user-defined fields\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-emsx/refs/heads/main/json-schema/bloomberg-emsx-route-schema.json
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
title: Bloomberg EMSX Route
---
