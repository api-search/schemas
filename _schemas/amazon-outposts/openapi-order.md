---
description: Information about an order.
layout: schema
name: Order
properties_list:
- description: ''
  name: OutpostId
  type: object
- description: ''
  name: OrderId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: LineItems
  type: object
- description: ''
  name: PaymentOption
  type: object
- description: ''
  name: OrderSubmissionDate
  type: object
- description: ''
  name: OrderFulfilledDate
  type: object
- description: ''
  name: PaymentTerm
  type: object
- description: ''
  name: OrderType
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-order-schema.json
slug: openapi-order
source_filename: openapi-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-order-schema.json\",\n  \"title\": \"Order\",\n  \"description\": \"Information about an order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutpostId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutpostIdOnly\"\n        },\n        {\n          \"description\": \" The ID of the Outpost in the order. \"\n        }\n      ]\n    },\n    \"OrderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderId\"\n        },\n        {\n          \"description\": \"The ID of the order.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the order.</p> <ul> <li> <p> <code>PREPARING</code>\
  \ - Order is received and being prepared.</p> </li> <li> <p> <code>IN_PROGRESS</code> - Order is either being built, shipped, or installed. To get more details, see the line item status.</p> </li> <li> <p> <code>COMPLETED</code> - Order is complete.</p> </li> <li> <p> <code>CANCELLED</code> - Order is cancelled.</p> </li> <li> <p> <code>ERROR</code> - Customer should contact support.</p> </li> </ul> <note> <p>The following status are deprecated: <code>RECEIVED</code>, <code>PENDING</code>, <code>PROCESSING</code>, <code>INSTALLING</code>, and <code>FULFILLED</code>. </p> </note>\"\n        }\n      ]\n    },\n    \"LineItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineItemListDefinition\"\n        },\n        {\n          \"description\": \"The line items for the order\"\n        }\n      ]\n    },\n    \"PaymentOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaymentOption\"\n        },\n        {\n        \
  \  \"description\": \"The payment option for the order.\"\n        }\n      ]\n    },\n    \"OrderSubmissionDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ISO8601Timestamp\"\n        },\n        {\n          \"description\": \"The submission date for the order.\"\n        }\n      ]\n    },\n    \"OrderFulfilledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ISO8601Timestamp\"\n        },\n        {\n          \"description\": \"The fulfillment date of the order.\"\n        }\n      ]\n    },\n    \"PaymentTerm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaymentTerm\"\n        },\n        {\n          \"description\": \"The payment term.\"\n        }\n      ]\n    },\n    \"OrderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderType\"\n        },\n        {\n          \"description\": \"The type of order.\"\n        }\n      ]\n    }\n \
  \ }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-order-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: Order
---
