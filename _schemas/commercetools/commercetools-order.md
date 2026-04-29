---
description: An order created from a cart upon successful checkout in a commercetools Composable Commerce project. Orders capture the immutable state of line items, pricing, addresses, and payment information at the time of purchase.
layout: schema
name: commercetools Order
properties_list:
- description: System-generated unique identifier for the order.
  name: id
  type: string
- description: Current version of the order resource for optimistic concurrency control.
  name: version
  type: integer
- description: User-defined unique key for the order.
  name: key
  type: string
- description: Human-readable order number, unique within the project.
  name: orderNumber
  type: string
- description: A purchase order number for business-to-business order references.
  name: purchaseOrderNumber
  type: string
- description: ID of the customer who placed the order.
  name: customerId
  type: string
- description: Email address of the customer at time of order creation.
  name: customerEmail
  type: string
- description: Customer group of the customer at time of order creation.
  name: customerGroup
  type: object
- description: Anonymous session ID for guest checkout orders.
  name: anonymousId
  type: string
- description: Business unit this order belongs to in B2B contexts.
  name: businessUnit
  type: object
- description: Store this order was placed in.
  name: store
  type: object
- description: Product line items captured at the time of order creation.
  name: lineItems
  type: array
- description: Custom line items with user-defined pricing captured at order creation.
  name: customLineItems
  type: array
- description: Total price of all line items and custom line items.
  name: totalPrice
  type: object
- description: Total price including tax breakdown, available when tax calculation is complete.
  name: taxedPrice
  type: object
- description: Tax calculation mode used for this order.
  name: taxMode
  type: string
- description: Rounding mode used for tax calculations.
  name: taxRoundingMode
  type: string
- description: Whether tax is calculated at line item or unit price level.
  name: taxCalculationMode
  type: string
- description: Inventory tracking mode applied to this order.
  name: inventoryMode
  type: string
- description: High-level lifecycle state of the order.
  name: orderState
  type: string
- description: Reference to a custom state machine state for the order.
  name: state
  type: object
- description: Current fulfillment state of the order.
  name: shipmentState
  type: string
- description: Current payment state of the order.
  name: paymentState
  type: string
- description: Billing address captured at order creation.
  name: billingAddress
  type: object
- description: Primary shipping address captured at order creation.
  name: shippingAddress
  type: object
- description: Shipping method and rate applied to the order.
  name: shippingInfo
  type: object
- description: References to payment resources associated with the order.
  name: paymentInfo
  type: object
- description: Discount codes applied to the order.
  name: discountCodes
  type: array
- description: Total number of line items in the order.
  name: lineItemCount
  type: integer
- description: Synchronization information for external system integrations.
  name: syncInfo
  type: array
- description: Return information including returned items and refund state.
  name: returnInfo
  type: array
- description: Delivery records tracking physical fulfillment of order items.
  name: deliveries
  type: array
- description: ISO 8601 timestamp when the order was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the order was last modified.
  name: lastModifiedAt
  type: string
- description: ISO 8601 timestamp when the order reached the Complete state.
  name: completedAt
  type: string
- description: Custom fields and type reference for extended order attributes.
  name: custom
  type: object
provider_name: commercetools
provider_slug: commercetools
schema_file: json-schema/commercetools-order-schema.json
slug: commercetools-order
source_filename: commercetools-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/schemas/commercetools/order.json\",\n  \"title\": \"commercetools Order\",\n  \"description\": \"An order created from a cart upon successful checkout in a commercetools Composable Commerce project. Orders capture the immutable state of line items, pricing, addresses, and payment information at the time of purchase.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"version\", \"orderState\", \"lineItems\", \"customLineItems\", \"totalPrice\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated unique identifier for the order.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Current version of the order resource for optimistic concurrency control.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"minLength\": 2,\n      \"maxLength\"\
  : 256,\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\",\n      \"description\": \"User-defined unique key for the order.\"\n    },\n    \"orderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable order number, unique within the project.\"\n    },\n    \"purchaseOrderNumber\": {\n      \"type\": \"string\",\n      \"description\": \"A purchase order number for business-to-business order references.\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the customer who placed the order.\"\n    },\n    \"customerEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the customer at time of order creation.\"\n    },\n    \"customerGroup\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Customer group of the customer at time of order creation.\"\n    },\n    \"anonymousId\": {\n      \"type\": \"string\",\n      \"description\": \"Anonymous session ID\
  \ for guest checkout orders.\"\n    },\n    \"businessUnit\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Business unit this order belongs to in B2B contexts.\"\n    },\n    \"store\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Store this order was placed in.\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LineItem\"\n      },\n      \"description\": \"Product line items captured at the time of order creation.\"\n    },\n    \"customLineItems\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomLineItem\"\n      },\n      \"description\": \"Custom line items with user-defined pricing captured at order creation.\"\n    },\n    \"totalPrice\": {\n      \"$ref\": \"#/$defs/Money\",\n      \"description\": \"Total price of all line items and custom line items.\"\n    },\n    \"taxedPrice\": {\n      \"$ref\": \"#/$defs/TaxedPrice\",\n      \"description\"\
  : \"Total price including tax breakdown, available when tax calculation is complete.\"\n    },\n    \"taxMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"Platform\", \"External\", \"ExternalAmount\", \"Disabled\"],\n      \"description\": \"Tax calculation mode used for this order.\"\n    },\n    \"taxRoundingMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"HalfEven\", \"HalfUp\", \"HalfDown\"],\n      \"description\": \"Rounding mode used for tax calculations.\"\n    },\n    \"taxCalculationMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"LineItemLevel\", \"UnitPriceLevel\"],\n      \"description\": \"Whether tax is calculated at line item or unit price level.\"\n    },\n    \"inventoryMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"None\", \"TrackOnly\", \"ReserveOnOrder\"],\n      \"description\": \"Inventory tracking mode applied to this order.\"\n    },\n    \"orderState\": {\n      \"type\": \"string\",\n      \"enum\": [\"Open\", \"Confirmed\"\
  , \"Complete\", \"Cancelled\"],\n      \"description\": \"High-level lifecycle state of the order.\"\n    },\n    \"state\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Reference to a custom state machine state for the order.\"\n    },\n    \"shipmentState\": {\n      \"type\": \"string\",\n      \"enum\": [\"Shipped\", \"Ready\", \"Pending\", \"Delayed\", \"Partial\", \"Backorder\"],\n      \"description\": \"Current fulfillment state of the order.\"\n    },\n    \"paymentState\": {\n      \"type\": \"string\",\n      \"enum\": [\"Paid\", \"Pending\", \"Failed\", \"CreditOwed\", \"BalanceDue\"],\n      \"description\": \"Current payment state of the order.\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"Billing address captured at order creation.\"\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"Primary shipping address captured at order creation.\"\n    },\n\
  \    \"shippingInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Shipping method and rate applied to the order.\"\n    },\n    \"paymentInfo\": {\n      \"type\": \"object\",\n      \"description\": \"References to payment resources associated with the order.\"\n    },\n    \"discountCodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Discount codes applied to the order.\"\n    },\n    \"lineItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of line items in the order.\"\n    },\n    \"syncInfo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Synchronization information for external system integrations.\"\n    },\n    \"returnInfo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ReturnInfo\"\n      },\n      \"description\": \"Return information including returned items\
  \ and refund state.\"\n    },\n    \"deliveries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Delivery\"\n      },\n      \"description\": \"Delivery records tracking physical fulfillment of order items.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the order was created.\"\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the order was last modified.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the order reached the Complete state.\"\n    },\n    \"custom\": {\n      \"type\": \"object\",\n      \"description\": \"Custom fields and type reference for extended order attributes.\"\n    }\n  },\n  \"$defs\": {\n    \"Reference\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A reference to another commercetools resource by type and ID.\",\n      \"required\": [\"typeId\", \"id\"],\n      \"properties\": {\n        \"typeId\": {\n          \"type\": \"string\",\n          \"description\": \"The type identifier of the referenced resource (e.g., 'product', 'customer').\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The system-generated unique identifier of the referenced resource.\"\n        }\n      }\n    },\n    \"Money\": {\n      \"type\": \"object\",\n      \"description\": \"A monetary value with currency code and amount in the smallest currency unit.\",\n      \"required\": [\"currencyCode\", \"centAmount\"],\n      \"properties\": {\n        \"currencyCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 three-letter currency code.\"\n        },\n        \"centAmount\": {\n          \"type\": \"integer\",\n\
  \          \"description\": \"Amount in the smallest indivisible unit of the currency (e.g., cents for USD).\"\n        },\n        \"fractionDigits\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 20,\n          \"description\": \"Number of fraction digits for the currency.\"\n        }\n      }\n    },\n    \"TaxedPrice\": {\n      \"type\": \"object\",\n      \"description\": \"A price with full tax breakdown including total gross, net, and per-rate tax portions.\",\n      \"required\": [\"totalNet\", \"totalGross\"],\n      \"properties\": {\n        \"totalNet\": {\n          \"$ref\": \"#/$defs/Money\",\n          \"description\": \"Total price excluding all taxes.\"\n        },\n        \"totalGross\": {\n          \"$ref\": \"#/$defs/Money\",\n          \"description\": \"Total price including all taxes.\"\n        },\n        \"taxPortions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n \
  \         },\n          \"description\": \"Breakdown of tax portions by rate and name.\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A postal address with country and optional structured fields.\",\n      \"required\": [\"country\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the address within the resource.\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"User-defined identifier for the address.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"minLength\": 2,\n          \"maxLength\": 2,\n          \"description\": \"ISO 3166-1 alpha-2 country code.\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the address recipient.\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"Last name of the address recipient.\"\n        },\n        \"company\": {\n          \"type\": \"string\",\n          \"description\": \"Company name for business addresses.\"\n        },\n        \"streetName\": {\n          \"type\": \"string\",\n          \"description\": \"Street name component of the address.\"\n        },\n        \"streetNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Street number component of the address.\"\n        },\n        \"additionalStreetInfo\": {\n          \"type\": \"string\",\n          \"description\": \"Apartment, suite, floor, or other secondary address information.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City of the address.\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"State, province, or region.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address associated with this postal address.\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number associated with this postal address.\"\n        }\n      }\n    },\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"description\": \"A product line item in an order capturing the product, variant, quantity, and pricing at checkout time.\",\n      \"required\": [\"id\", \"productId\", \"name\", \"variant\", \"price\", \"totalPrice\", \"quantity\", \"lineItemMode\", \"priceMode\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the line item within the order.\"\n        },\n        \"productId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the product\
  \ this line item references.\"\n        },\n        \"productKey\": {\n          \"type\": \"string\",\n          \"description\": \"Key of the product at time of order creation.\"\n        },\n        \"name\": {\n          \"type\": \"object\",\n          \"description\": \"Localized name of the product at time of order creation.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Quantity of this product variant ordered.\"\n        },\n        \"price\": {\n          \"type\": \"object\",\n          \"description\": \"The unit price applied to this line item.\"\n        },\n        \"totalPrice\": {\n          \"$ref\": \"#/$defs/Money\",\n          \"description\": \"Total price for this line item (unit price multiplied by quantity).\"\n        },\n        \"lineItemMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"Standard\", \"GiftLineItem\"],\n          \"description\": \"Whether this\
  \ is a standard or complimentary gift line item.\"\n        },\n        \"priceMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"Platform\", \"ExternalTotal\", \"ExternalPrice\"],\n          \"description\": \"How the price for this line item was determined.\"\n        },\n        \"discountedPricePerQuantity\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"Discounted price information per unit quantity.\"\n        },\n        \"taxRate\": {\n          \"type\": \"object\",\n          \"description\": \"Tax rate applied to this line item.\"\n        }\n      }\n    },\n    \"CustomLineItem\": {\n      \"type\": \"object\",\n      \"description\": \"A custom-priced line item not linked to a product catalog entry.\",\n      \"required\": [\"id\", \"name\", \"money\", \"totalPrice\", \"quantity\", \"slug\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Unique identifier for the custom line item.\"\n        },\n        \"name\": {\n          \"type\": \"object\",\n          \"description\": \"Localized name of the custom line item.\"\n        },\n        \"money\": {\n          \"$ref\": \"#/$defs/Money\",\n          \"description\": \"Unit price of the custom line item.\"\n        },\n        \"totalPrice\": {\n          \"$ref\": \"#/$defs/Money\",\n          \"description\": \"Total price (money multiplied by quantity).\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"User-defined identifier for the custom line item type.\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Quantity of this custom line item.\"\n        }\n      }\n    },\n    \"Delivery\": {\n      \"type\": \"object\",\n      \"description\": \"A delivery record tracking physical fulfillment of order line items.\"\
  ,\n      \"required\": [\"id\", \"items\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the delivery.\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"User-defined key for the delivery.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the delivery was created.\"\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"Line items and quantities included in this delivery.\"\n        },\n        \"parcels\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Parcel\"\n          },\n          \"description\": \"Physical parcels within this delivery with tracking information.\"\n        },\n      \
  \  \"address\": {\n          \"$ref\": \"#/$defs/Address\",\n          \"description\": \"Delivery address for this delivery if different from the order shipping address.\"\n        }\n      }\n    },\n    \"Parcel\": {\n      \"type\": \"object\",\n      \"description\": \"A physical parcel within a delivery with tracking and measurement details.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the parcel.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the parcel was created.\"\n        },\n        \"measurements\": {\n          \"type\": \"object\",\n          \"description\": \"Physical dimensions and weight of the parcel.\"\n        },\n        \"trackingData\": {\n          \"type\": \"object\",\n          \"description\": \"Carrier tracking information\
  \ including tracking ID, carrier name, and URL.\"\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"Line items and quantities packed in this parcel.\"\n        }\n      }\n    },\n    \"ReturnInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Return information for items being returned from an order.\",\n      \"required\": [\"items\"],\n      \"properties\": {\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"Items being returned with quantities and return state.\"\n        },\n        \"returnTrackingId\": {\n          \"type\": \"string\",\n          \"description\": \"Tracking ID for the return shipment.\"\n        },\n        \"returnDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date\
  \ the return was initiated.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/json-schema/commercetools-order-schema.json
tags:
- Commerce
- Composable Commerce
- E-Commerce
- GraphQL
- REST
- SDK
title: commercetools Order
---
