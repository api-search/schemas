---
description: Schema for SAP S/4HANA Outbound Delivery Header entity (A_OutbDeliveryHeader) from the API_OUTBOUND_DELIVERY_SRV OData service. Represents a delivery document for shipping goods to customers.
layout: schema
name: SAP Outbound Delivery
properties_list:
- description: Delivery document number
  name: DeliveryDocument
  type: string
- description: Delivery type
  name: DeliveryDocumentType
  type: string
- description: Sold-to party
  name: SoldToParty
  type: string
- description: Ship-to party
  name: ShipToParty
  type: string
- description: Shipping point / receiving point
  name: ShippingPoint
  type: string
- description: Planned delivery date
  name: DeliveryDate
  type: string
- description: Route
  name: ActualDeliveryRoute
  type: string
- description: Date the delivery was created
  name: CreationDate
  type: string
- description: Actual goods movement date
  name: ActualGoodsMovementDate
  type: string
- description: Complete delivery flag
  name: CompleteDeliveryIsDefined
  type: boolean
- description: Overall goods movement status (A=Not yet started, B=Partially complete, C=Complete)
  name: OverallGoodsMovementStatus
  type: string
- description: Overall picking status
  name: OverallPickingStatus
  type: string
- description: Overall packing status
  name: OverallPackingStatus
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-outbound-delivery-schema.json
slug: sap-sd-outbound-delivery
source_filename: sap-sd-outbound-delivery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-outbound-delivery\",\n  \"title\": \"SAP Outbound Delivery\",\n  \"description\": \"Schema for SAP S/4HANA Outbound Delivery Header entity (A_OutbDeliveryHeader) from the API_OUTBOUND_DELIVERY_SRV OData service. Represents a delivery document for shipping goods to customers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryDocument\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Delivery document number\"\n    },\n    \"DeliveryDocumentType\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Delivery type\"\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Sold-to party\"\n    },\n    \"ShipToParty\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Ship-to party\"\n    },\n    \"\
  ShippingPoint\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Shipping point / receiving point\"\n    },\n    \"DeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Planned delivery date\"\n    },\n    \"ActualDeliveryRoute\": {\n      \"type\": \"string\",\n      \"maxLength\": 6,\n      \"description\": \"Route\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the delivery was created\"\n    },\n    \"ActualGoodsMovementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Actual goods movement date\"\n    },\n    \"CompleteDeliveryIsDefined\": {\n      \"type\": \"boolean\",\n      \"description\": \"Complete delivery flag\"\n    },\n    \"OverallGoodsMovementStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall goods movement status (A=Not\
  \ yet started, B=Partially complete, C=Complete)\"\n    },\n    \"OverallPickingStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall picking status\"\n    },\n    \"OverallPackingStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall packing status\"\n    }\n  },\n  \"required\": [\"DeliveryDocument\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-outbound-delivery-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Outbound Delivery
---
