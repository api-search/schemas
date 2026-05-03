---
description: Schema for an Oracle Transportation Management shipment order (order to move), representing a request to transport goods from one location to another.
layout: schema
name: Oracle OTM Shipment Order
properties_list:
- description: Global identifier in domain.xid format
  name: shipmentOrderGid
  type: string
- description: User-defined order identifier
  name: shipmentOrderXid
  type: string
- description: I=Initial, OB=Open-Booked, PL=Planned, DP=Dispatched, IT=InTransit, DL=Delivered, CL=Closed
  name: status
  type: string
- description: Origin location GID
  name: sourceLocationGid
  type: string
- description: Destination location GID
  name: destLocationGid
  type: string
- description: Earliest allowable pickup date
  name: earlyPickupDate
  type: string
- description: Latest allowable pickup date
  name: latePickupDate
  type: string
- description: ''
  name: earlyDeliveryDate
  type: string
- description: Required delivery date
  name: lateDeliveryDate
  type: string
- description: ''
  name: transportationMode
  type: string
- description: Total shipment weight
  name: totalWeight
  type: number
- description: Weight unit of measure
  name: totalWeightUom
  type: string
- description: ''
  name: totalVolume
  type: number
- description: ''
  name: totalVolumeUom
  type: string
- description: Shipment order line items
  name: lines
  type: array
- description: ''
  name: insertDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle Transportation Management
provider_slug: oracle-transportation-management
schema_file: json-schema/oracle-otm-shipment-order-schema.json
slug: oracle-otm-shipment-order
source_filename: oracle-otm-shipment-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/oracle-transportation-management/json-schema/oracle-otm-shipment-order-schema.json\",\n  \"title\": \"Oracle OTM Shipment Order\",\n  \"description\": \"Schema for an Oracle Transportation Management shipment order (order to move), representing a request to transport goods from one location to another.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shipmentOrderGid\": {\n      \"type\": \"string\",\n      \"description\": \"Global identifier in domain.xid format\"\n    },\n    \"shipmentOrderXid\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined order identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"I\", \"OB\", \"PL\", \"DP\", \"IT\", \"DL\", \"CL\"],\n      \"description\": \"I=Initial, OB=Open-Booked, PL=Planned, DP=Dispatched, IT=InTransit, DL=Delivered, CL=Closed\"\n    },\n    \"sourceLocationGid\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Origin location GID\"\n    },\n    \"destLocationGid\": {\n      \"type\": \"string\",\n      \"description\": \"Destination location GID\"\n    },\n    \"earlyPickupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Earliest allowable pickup date\"\n    },\n    \"latePickupDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Latest allowable pickup date\"\n    },\n    \"earlyDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lateDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Required delivery date\"\n    },\n    \"transportationMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"LTL\", \"TL\", \"OCEAN\", \"AIR\", \"RAIL\", \"PARCEL\", \"INTERMODAL\"]\n    },\n    \"totalWeight\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Total shipment weight\"\n    },\n    \"totalWeightUom\": {\n      \"type\": \"string\",\n      \"enum\": [\"LB\", \"KG\", \"T\", \"MT\"],\n      \"description\": \"Weight unit of measure\"\n    },\n    \"totalVolume\": {\n      \"type\": \"number\"\n    },\n    \"totalVolumeUom\": {\n      \"type\": \"string\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"Shipment order line items\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ShipmentOrderLine\"\n      }\n    },\n    \"insertDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"shipmentOrderXid\", \"sourceLocationGid\", \"destLocationGid\", \"lateDeliveryDate\"],\n  \"$defs\": {\n    \"ShipmentOrderLine\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lineNumber\": { \"type\": \"integer\" },\n        \"itemGid\": { \"type\": \"\
  string\" },\n        \"itemDescription\": { \"type\": \"string\" },\n        \"quantity\": { \"type\": \"number\" },\n        \"quantityUom\": { \"type\": \"string\" },\n        \"weight\": { \"type\": \"number\" },\n        \"weightUom\": { \"type\": \"string\", \"enum\": [\"LB\", \"KG\", \"T\", \"MT\"] },\n        \"volume\": { \"type\": \"number\" },\n        \"volumeUom\": { \"type\": \"string\" },\n        \"packageType\": { \"type\": \"string\" }\n      },\n      \"required\": [\"lineNumber\", \"quantity\", \"quantityUom\"]\n    }\n  },\n  \"examples\": [\n    {\n      \"shipmentOrderXid\": \"SO-2026-00456\",\n      \"shipmentOrderGid\": \"ACME.SO-2026-00456\",\n      \"status\": \"PL\",\n      \"sourceLocationGid\": \"ACME.CHICAGO-WH\",\n      \"destLocationGid\": \"ACME.DALLAS-DC\",\n      \"earlyPickupDate\": \"2026-03-20T07:00:00Z\",\n      \"latePickupDate\": \"2026-03-20T17:00:00Z\",\n      \"earlyDeliveryDate\": \"2026-03-22T07:00:00Z\",\n      \"lateDeliveryDate\": \"2026-03-22T17:00:00Z\"\
  ,\n      \"transportationMode\": \"TL\",\n      \"totalWeight\": 42000,\n      \"totalWeightUom\": \"LB\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-transportation-management/refs/heads/main/json-schema/oracle-otm-shipment-order-schema.json
tags:
- Logistics
- Transportation
- Freight
- Supply Chain
- Shipping
- Global Trade
- Oracle
title: Oracle OTM Shipment Order
---
