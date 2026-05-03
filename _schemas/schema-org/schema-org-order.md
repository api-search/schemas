---
description: An order is a confirmation of a transaction, typically from an online shop.
layout: schema
name: Schema.org Order
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The identifier of the transaction.
  name: orderNumber
  type: string
- description: The current status of the order.
  name: orderStatus
  type: string
- description: Date order was placed.
  name: orderDate
  type: string
- description: Party placing the order.
  name: customer
  type: object
- description: An entity which offers goods or services.
  name: seller
  type: object
- description: An entity that arranges for the exchange.
  name: broker
  type: object
- description: The item ordered.
  name: orderedItem
  type: object
- description: The offer(s) that were accepted as part of this order.
  name: acceptedOffer
  type: object
- description: The billing address for the order.
  name: billingAddress
  type: object
- description: The name of the credit card or other method of payment for the order.
  name: paymentMethod
  type: string
- description: An identifier for the method of payment used.
  name: paymentMethodId
  type: string
- description: The URL for sending a payment.
  name: paymentUrl
  type: string
- description: The date that payment is due.
  name: paymentDueDate
  type: string
- description: Any discount applied to the order.
  name: discount
  type: object
- description: Code used to redeem a discount.
  name: discountCode
  type: string
- description: The currency of the discount.
  name: discountCurrency
  type: string
- description: Was the offer accepted as a gift for someone other than the buyer.
  name: isGift
  type: boolean
- description: The delivery of the parcel related to this order.
  name: orderDelivery
  type: object
- description: A number confirming the given order.
  name: confirmationNumber
  type: string
- description: URL of the order.
  name: url
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-order-schema.json
slug: schema-org-order
source_filename: schema-org-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/order.json\",\n  \"title\": \"Schema.org Order\",\n  \"description\": \"An order is a confirmation of a transaction, typically from an online shop.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"Order\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"orderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the transaction.\"\n    },\n    \"orderStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"OrderCancelled\", \"OrderDelivered\", \"OrderInTransit\", \"OrderPaymentDue\", \"OrderPickupAvailable\", \"OrderProblem\", \"OrderProcessing\", \"OrderReturned\"],\n      \"description\": \"The current status of the order.\"\
  \n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date order was placed.\"\n    },\n    \"customer\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"Party placing the order.\"\n    },\n    \"seller\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"An entity which offers goods or services.\"\n    },\n    \"broker\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"An entity that arranges for the exchange.\"\n    },\n    \"orderedItem\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/OrderItem\" },\n        { \"type\": \"array\"\
  , \"items\": { \"$ref\": \"#/$defs/OrderItem\" } },\n        { \"$ref\": \"schema-org-product-schema.json\" }\n      ],\n      \"description\": \"The item ordered.\"\n    },\n    \"acceptedOffer\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"The offer(s) that were accepted as part of this order.\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"schema-org-postal-address-schema.json\",\n      \"description\": \"The billing address for the order.\"\n    },\n    \"paymentMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the credit card or other method of payment for the order.\"\n    },\n    \"paymentMethodId\": {\n      \"type\": \"string\",\n      \"description\": \"An identifier for the method of payment used.\"\n    },\n    \"paymentUrl\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uri\",\n      \"description\": \"The URL for sending a payment.\"\n    },\n    \"paymentDueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date that payment is due.\"\n    },\n    \"discount\": {\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" }\n      ],\n      \"description\": \"Any discount applied to the order.\"\n    },\n    \"discountCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code used to redeem a discount.\"\n    },\n    \"discountCurrency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"The currency of the discount.\"\n    },\n    \"isGift\": {\n      \"type\": \"boolean\",\n      \"description\": \"Was the offer accepted as a gift for someone other than the buyer.\"\n    },\n    \"orderDelivery\": {\n      \"$ref\": \"#/$defs/ParcelDelivery\",\n      \"description\": \"The delivery of the parcel related to this order.\"\
  \n    },\n    \"confirmationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"A number confirming the given order.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the order.\"\n    }\n  },\n  \"$defs\": {\n    \"OrderItem\": {\n      \"type\": \"object\",\n      \"description\": \"An order item is a line of an order.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"OrderItem\" },\n        \"orderItemNumber\": { \"type\": \"string\", \"description\": \"The identifier of the order item.\" },\n        \"orderQuantity\": { \"type\": \"integer\", \"description\": \"The number of the item ordered.\" },\n        \"orderItemStatus\": { \"type\": \"string\", \"enum\": [\"OrderCancelled\", \"OrderDelivered\", \"OrderInTransit\", \"OrderPaymentDue\", \"OrderPickupAvailable\", \"OrderProblem\", \"OrderProcessing\", \"OrderReturned\"], \"description\": \"The current status of the\
  \ order item.\" },\n        \"orderedItem\": { \"type\": \"object\", \"properties\": { \"@type\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } }, \"description\": \"The item ordered.\" }\n      }\n    },\n    \"ParcelDelivery\": {\n      \"type\": \"object\",\n      \"description\": \"The delivery of a parcel.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"ParcelDelivery\" },\n        \"trackingNumber\": { \"type\": \"string\", \"description\": \"Shipper tracking number.\" },\n        \"trackingUrl\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Tracking URL for the parcel delivery.\" },\n        \"deliveryStatus\": { \"type\": \"string\", \"description\": \"New entry added as the package is delivered.\" },\n        \"expectedArrivalFrom\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"The earliest date the package may arrive.\" },\n        \"expectedArrivalUntil\": { \"type\": \"string\",\
  \ \"format\": \"date-time\", \"description\": \"The latest date the package may arrive.\" },\n        \"carrier\": { \"$ref\": \"schema-org-organization-schema.json\", \"description\": \"The party responsible for the parcel delivery.\" },\n        \"deliveryAddress\": { \"$ref\": \"schema-org-postal-address-schema.json\", \"description\": \"Destination address.\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-order-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Order
---
