---
description: A trade execution record within Bloomberg AIM/EMSX, representing a route sent to a broker and its associated fills. Maps to the EMSX route concept with embedded fill data.
layout: schema
name: Trade
properties_list:
- description: Parent order sequence number in EMSX
  name: sequenceNumber
  type: integer
- description: Unique route identifier within the parent order
  name: routeId
  type: integer
- description: Bloomberg ticker of the traded security
  name: ticker
  type: string
- description: Trade direction
  name: side
  type: string
- description: Quantity routed to the broker
  name: amount
  type: integer
- description: Quantity filled on this route
  name: filledAmount
  type: integer
- description: Volume-weighted average fill price for this route
  name: averagePrice
  type: number
- description: Broker code the route was sent to
  name: broker
  type: string
- description: Order type for this route
  name: orderType
  type: string
- description: Limit price sent with the route
  name: limitPrice
  type: number
- description: Stop price sent with the route
  name: stopPrice
  type: number
- description: Time in force for this route
  name: timeInForce
  type: string
- description: Broker execution strategy name
  name: strategy
  type: string
- description: Strategy-specific parameters sent to the broker
  name: strategyParameters
  type: object
- description: Free-text execution instructions for the broker
  name: executionInstructions
  type: string
- description: Current route status
  name: status
  type: string
- description: Trading account used for this route
  name: account
  type: string
- description: Exchange where execution occurred
  name: exchange
  type: string
- description: Commission charged for this route execution
  name: commission
  type: number
- description: How commission is calculated
  name: commissionType
  type: string
- description: Net monetary amount of the trade (quantity x avgPrice +/- commission)
  name: netAmount
  type: number
- description: Expected or actual settlement date
  name: settlementDate
  type: string
- description: Individual fill records for this route
  name: fills
  type: array
- description: Date the route was created
  name: createdDate
  type: string
- description: Time the route was created (HH:MM:SS)
  name: createdTime
  type: string
- description: Date of the most recent fill
  name: lastFillDate
  type: string
- description: Time of the most recent fill (HH:MM:SS)
  name: lastFillTime
  type: string
- description: Timestamp of the last route update
  name: lastUpdated
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/trade.json
slug: trade
source_filename: trade.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://bloomberg.com/schemas/trade.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Trade\",\n  \"description\": \"A trade execution record within Bloomberg AIM/EMSX, representing a route sent to a broker and its associated fills. Maps to the EMSX route concept with embedded fill data.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sequenceNumber\",\n    \"routeId\",\n    \"ticker\",\n    \"side\",\n    \"amount\",\n    \"broker\"\n  ],\n  \"properties\": {\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent order sequence number in EMSX\"\n    },\n    \"routeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique route identifier within the parent order\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg ticker of the traded security\",\n      \"examples\": [\n        \"IBM US Equity\",\n        \"AAPL US Equity\"\n\
  \      ]\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Trade direction\",\n      \"enum\": [\n        \"BUY\",\n        \"SELL\",\n        \"SHRT\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity routed to the broker\",\n      \"minimum\": 1\n    },\n    \"filledAmount\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity filled on this route\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"averagePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Volume-weighted average fill price for this route\"\n    },\n    \"broker\": {\n      \"type\": \"string\",\n      \"description\": \"Broker code the route was sent to\"\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"description\": \"Order type for this route\",\n      \"enum\": [\n        \"MKT\",\n        \"LMT\",\n        \"STP\",\n        \"STP LMT\"\n      ]\n    },\n    \"limitPrice\":\
  \ {\n      \"type\": \"number\",\n      \"description\": \"Limit price sent with the route\"\n    },\n    \"stopPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Stop price sent with the route\"\n    },\n    \"timeInForce\": {\n      \"type\": \"string\",\n      \"description\": \"Time in force for this route\",\n      \"enum\": [\n        \"DAY\",\n        \"GTC\",\n        \"OPG\",\n        \"IOC\",\n        \"FOK\",\n        \"GTD\",\n        \"MOC\",\n        \"LOC\"\n      ]\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"description\": \"Broker execution strategy name\"\n    },\n    \"strategyParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Strategy-specific parameters sent to the broker\",\n      \"additionalProperties\": true\n    },\n    \"executionInstructions\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text execution instructions for the broker\"\n    },\n    \"status\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Current route status\",\n      \"enum\": [\n        \"CANCEL\",\n        \"CXL_PND\",\n        \"DONE\",\n        \"FILL\",\n        \"MOD_PND\",\n        \"NEW\",\n        \"PART_FILL\",\n        \"RJCT\",\n        \"SENT\",\n        \"WORKING\"\n      ]\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Trading account used for this route\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange where execution occurred\"\n    },\n    \"commission\": {\n      \"type\": \"number\",\n      \"description\": \"Commission charged for this route execution\"\n    },\n    \"commissionType\": {\n      \"type\": \"string\",\n      \"description\": \"How commission is calculated\",\n      \"enum\": [\n        \"PerShare\",\n        \"Percentage\",\n        \"Fixed\"\n      ]\n    },\n    \"netAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Net monetary amount of the trade (quantity\
  \ x avgPrice +/- commission)\"\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expected or actual settlement date\"\n    },\n    \"fills\": {\n      \"type\": \"array\",\n      \"description\": \"Individual fill records for this route\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Fill\"\n      }\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the route was created\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time the route was created (HH:MM:SS)\"\n    },\n    \"lastFillDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the most recent fill\"\n    },\n    \"lastFillTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time of the most recent fill (HH:MM:SS)\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Timestamp of the last route update\"\n    }\n  },\n  \"$defs\": {\n    \"Fill\": {\n      \"type\": \"object\",\n      \"description\": \"An individual fill (partial or complete execution) within a route\",\n      \"required\": [\n        \"fillId\",\n        \"fillAmount\",\n        \"fillPrice\"\n      ],\n      \"properties\": {\n        \"fillId\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique fill identifier\"\n        },\n        \"fillAmount\": {\n          \"type\": \"integer\",\n          \"description\": \"Quantity executed in this fill\",\n          \"minimum\": 1\n        },\n        \"fillPrice\": {\n          \"type\": \"number\",\n          \"description\": \"Execution price for this fill\"\n        },\n        \"fillDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date of the fill\"\n        },\n        \"fillTime\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Time of the fill (HH:MM:SS)\"\n        },\n        \"exchange\": {\n          \"type\": \"string\",\n          \"description\": \"Exchange where the fill occurred\"\n        },\n        \"broker\": {\n          \"type\": \"string\",\n          \"description\": \"Broker that executed the fill\"\n        },\n        \"isManual\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this fill was manually entered\",\n          \"default\": false\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/trade.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Trade
---
