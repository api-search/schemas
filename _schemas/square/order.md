---
description: Contains all information related to a single order to process with Square, including line items that specify the products to purchase. Order objects also include information about any associated tenders, refunds, and returns.
layout: schema
name: Square Order
properties_list:
- description: The order's unique ID.
  name: id
  type: string
- description: The ID of the seller location that this order is associated with.
  name: location_id
  type: string
- description: A client-specified ID to associate an entity in another system with this order.
  name: reference_id
  type: string
- description: The origination details of the order.
  name: source
  type: object
- description: The ID of the customer associated with the order.
  name: customer_id
  type: string
- description: The line items included in the order.
  name: line_items
  type: array
- description: The list of all taxes associated with the order.
  name: taxes
  type: array
- description: The list of all discounts associated with the order.
  name: discounts
  type: array
- description: A list of service charges applied to the order.
  name: service_charges
  type: array
- description: Details about order fulfillment.
  name: fulfillments
  type: array
- description: A collection of items from sale orders being returned in this one.
  name: returns
  type: array
- description: The rollup of the returned money amounts.
  name: return_amounts
  type: object
- description: The net money amounts (sale money - return money).
  name: net_amounts
  type: object
- description: A positive rounding adjustment to the total of the order.
  name: rounding_adjustment
  type: object
- description: The tenders that were used to pay for the order.
  name: tenders
  type: array
- description: The refunds that are part of this order.
  name: refunds
  type: array
- description: Application-defined data attached to this order. Metadata fields are intended to store descriptive references or associations with an entity in another system.
  name: metadata
  type: object
- description: The timestamp for when the order was created, in RFC 3339 format.
  name: created_at
  type: string
- description: The timestamp for when the order was last updated, in RFC 3339 format.
  name: updated_at
  type: string
- description: The timestamp for when the order reached a terminal state, in RFC 3339 format.
  name: closed_at
  type: string
- description: The current state of the order.
  name: state
  type: string
- description: The version number, incremented each time an update is committed to the order.
  name: version
  type: integer
- description: The total amount of money to collect for the order.
  name: total_money
  type: object
- description: The total amount of tax money to collect for the order.
  name: total_tax_money
  type: object
- description: The total amount of discount money to collect for the order.
  name: total_discount_money
  type: object
- description: The total amount of tip money to collect for the order.
  name: total_tip_money
  type: object
- description: The total amount of service charge money to collect for the order.
  name: total_service_charge_money
  type: object
- description: A short-term identifier for the order used on receipts, the Seller Dashboard, and the Point of Sale device.
  name: ticket_name
  type: string
- description: Pricing options for an order.
  name: pricing_options
  type: object
provider_name: Square
provider_slug: square
schema_file: json-schema/order.json
slug: order
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/square/blob/main/json-schema/order.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Square Order\",\n  \"description\": \"Contains all information related to a single order to process with Square, including line items that specify the products to purchase. Order objects also include information about any associated tenders, refunds, and returns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The order's unique ID.\",\n      \"readOnly\": true\n    },\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the seller location that this order is associated with.\",\n      \"minLength\": 1\n    },\n    \"reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"A client-specified ID to associate an entity in another system with this order.\",\n      \"maxLength\": 40\n\
  \    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The origination details of the order.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name used to identify the place (application, device, etc.) that created the order.\"\n        }\n      }\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the customer associated with the order.\",\n      \"maxLength\": 191\n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"A unique ID that identifies the line item only within this order.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the line item.\"\n          },\n          \"quantity\": {\n            \"type\": \"\
  string\",\n            \"description\": \"The quantity purchased, as a string representation of a number.\"\n          },\n          \"catalog_object_id\": {\n            \"type\": \"string\",\n            \"description\": \"The catalog object ID for the item or item variation.\"\n          },\n          \"catalog_version\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The version of the catalog object that this line item references.\"\n          },\n          \"variation_name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the variation applied to this line item.\"\n          },\n          \"note\": {\n            \"type\": \"string\",\n            \"description\": \"The note of the line item.\"\n          },\n          \"base_price_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The base price for a single unit of the line item.\"\n          },\n        \
  \  \"gross_sales_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The gross sales amount of money calculated as (item base price) * quantity.\",\n            \"readOnly\": true\n          },\n          \"total_tax_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The total tax amount of money to collect for the line item.\",\n            \"readOnly\": true\n          },\n          \"total_discount_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The total discount amount of money to collect for the line item.\",\n            \"readOnly\": true\n          },\n          \"total_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The total amount of money to collect for this line item.\",\n            \"readOnly\": true\n          },\n          \"applied_taxes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n\
  \              \"properties\": {\n                \"tax_uid\": {\n                  \"type\": \"string\",\n                  \"description\": \"The uid of the tax for which this applied tax represents.\"\n                },\n                \"applied_money\": {\n                  \"$ref\": \"money.json\",\n                  \"description\": \"The amount of money applied by the tax to the line item.\"\n                }\n              }\n            },\n            \"description\": \"The list of taxes applied to this line item.\"\n          },\n          \"applied_discounts\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"discount_uid\": {\n                  \"type\": \"string\",\n                  \"description\": \"The uid of the discount for which this applied discount represents.\"\n                },\n                \"applied_money\": {\n                  \"$ref\": \"money.json\"\
  ,\n                  \"description\": \"The amount of money applied by the discount to the line item.\"\n                }\n              }\n            },\n            \"description\": \"The list of discounts applied to this line item.\"\n          },\n          \"item_type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of line item: an itemized sale, a non-itemized sale, or a custom amount.\",\n            \"enum\": [\"ITEM\", \"CUSTOM_AMOUNT\", \"GIFT_CARD\"]\n          },\n          \"metadata\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Application-defined data attached to this line item.\"\n          }\n        },\n        \"required\": [\"quantity\"]\n      },\n      \"description\": \"The line items included in the order.\"\n    },\n    \"taxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"A unique ID that identifies the tax only within this order.\"\n          },\n          \"catalog_object_id\": {\n            \"type\": \"string\",\n            \"description\": \"The catalog object ID referencing a CatalogTax.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The tax's name.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Indicates the calculation method used to apply the tax.\",\n            \"enum\": [\"INCLUSIVE\", \"ADDITIVE\", \"UNKNOWN_TAX\"]\n          },\n          \"percentage\": {\n            \"type\": \"string\",\n            \"description\": \"The percentage of the tax, as a string representation of a decimal number.\"\n          },\n          \"scope\": {\n            \"type\": \"string\",\n            \"description\": \"Indicates\
  \ whether the tax is scoped to the entire order or a single line item.\",\n            \"enum\": [\"OTHER_TAX_SCOPE\", \"ORDER\", \"LINE_ITEM\"]\n          },\n          \"applied_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The amount of money applied by the tax in the order.\",\n            \"readOnly\": true\n          }\n        }\n      },\n      \"description\": \"The list of all taxes associated with the order.\"\n    },\n    \"discounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"A unique ID that identifies the discount only within this order.\"\n          },\n          \"catalog_object_id\": {\n            \"type\": \"string\",\n            \"description\": \"The catalog object ID referencing a CatalogDiscount.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n \
  \           \"description\": \"The discount's name.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of discount.\",\n            \"enum\": [\"FIXED_PERCENTAGE\", \"FIXED_AMOUNT\", \"VARIABLE_PERCENTAGE\", \"VARIABLE_AMOUNT\"]\n          },\n          \"percentage\": {\n            \"type\": \"string\",\n            \"description\": \"The percentage of the discount, as a string representation of a decimal number.\"\n          },\n          \"amount_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The fixed amount of the discount.\"\n          },\n          \"applied_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The amount of money applied by the discount in the order.\",\n            \"readOnly\": true\n          },\n          \"scope\": {\n            \"type\": \"string\",\n            \"description\": \"Indicates whether the discount is scoped to the\
  \ entire order or a single line item.\",\n            \"enum\": [\"OTHER_DISCOUNT_SCOPE\", \"ORDER\", \"LINE_ITEM\"]\n          }\n        }\n      },\n      \"description\": \"The list of all discounts associated with the order.\"\n    },\n    \"service_charges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"A unique ID that identifies the service charge only within this order.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the service charge.\"\n          },\n          \"catalog_object_id\": {\n            \"type\": \"string\",\n            \"description\": \"The catalog object ID referencing the service charge.\"\n          },\n          \"percentage\": {\n            \"type\": \"string\",\n            \"description\": \"The service charge percentage as a string representation\
  \ of a decimal number.\"\n          },\n          \"amount_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The amount of a non-percentage-based service charge.\"\n          },\n          \"total_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The total amount of money to collect for the service charge.\",\n            \"readOnly\": true\n          }\n        }\n      },\n      \"description\": \"A list of service charges applied to the order.\"\n    },\n    \"fulfillments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"A unique ID that identifies the fulfillment only within this order.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of fulfillment.\",\n            \"enum\": [\"PICKUP\", \"SHIPMENT\", \"\
  DELIVERY\", \"DIGITAL\"]\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current state of the fulfillment.\",\n            \"enum\": [\"PROPOSED\", \"RESERVED\", \"PREPARED\", \"COMPLETED\", \"CANCELED\", \"FAILED\"]\n          }\n        }\n      },\n      \"description\": \"Details about order fulfillment.\"\n    },\n    \"returns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A collection of items from sale orders being returned.\"\n      },\n      \"description\": \"A collection of items from sale orders being returned in this one.\",\n      \"readOnly\": true\n    },\n    \"return_amounts\": {\n      \"type\": \"object\",\n      \"description\": \"The rollup of the returned money amounts.\",\n      \"readOnly\": true\n    },\n    \"net_amounts\": {\n      \"type\": \"object\",\n      \"description\": \"The net money amounts (sale money - return money).\",\n\
  \      \"readOnly\": true\n    },\n    \"rounding_adjustment\": {\n      \"type\": \"object\",\n      \"description\": \"A positive rounding adjustment to the total of the order.\",\n      \"readOnly\": true\n    },\n    \"tenders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A tender represents a payment method used in a transaction.\"\n      },\n      \"description\": \"The tenders that were used to pay for the order.\",\n      \"readOnly\": true\n    },\n    \"refunds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A refund associated with the order.\"\n      },\n      \"description\": \"The refunds that are part of this order.\",\n      \"readOnly\": true\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Application-defined data attached to this order.\
  \ Metadata fields are intended to store descriptive references or associations with an entity in another system.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp for when the order was created, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp for when the order was last updated, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"closed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp for when the order reached a terminal state, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the order.\",\n      \"enum\": [\"OPEN\", \"COMPLETED\", \"CANCELED\", \"DRAFT\"],\n      \"readOnly\": true\n    },\n  \
  \  \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number, incremented each time an update is committed to the order.\",\n      \"readOnly\": true\n    },\n    \"total_money\": {\n      \"$ref\": \"money.json\",\n      \"description\": \"The total amount of money to collect for the order.\",\n      \"readOnly\": true\n    },\n    \"total_tax_money\": {\n      \"$ref\": \"money.json\",\n      \"description\": \"The total amount of tax money to collect for the order.\",\n      \"readOnly\": true\n    },\n    \"total_discount_money\": {\n      \"$ref\": \"money.json\",\n      \"description\": \"The total amount of discount money to collect for the order.\",\n      \"readOnly\": true\n    },\n    \"total_tip_money\": {\n      \"$ref\": \"money.json\",\n      \"description\": \"The total amount of tip money to collect for the order.\",\n      \"readOnly\": true\n    },\n    \"total_service_charge_money\": {\n      \"$ref\": \"money.json\",\n      \"description\"\
  : \"The total amount of service charge money to collect for the order.\",\n      \"readOnly\": true\n    },\n    \"ticket_name\": {\n      \"type\": \"string\",\n      \"description\": \"A short-term identifier for the order used on receipts, the Seller Dashboard, and the Point of Sale device.\"\n    },\n    \"pricing_options\": {\n      \"type\": \"object\",\n      \"description\": \"Pricing options for an order.\",\n      \"properties\": {\n        \"auto_apply_discounts\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether automatic discounts are applied.\"\n        },\n        \"auto_apply_taxes\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether automatic taxes are applied.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"location_id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/square/refs/heads/main/json-schema/order.json
tags:
- Bookings
- Catalog
- Checkout
- Customers
- Disputes
- Ecommerce
- Financial Technology
- Gift Cards
- Inventory
- Invoicing
- Labor
- Locations
- Loyalty
- Merchants
- Orders
- Payments
- Point of Sale
- Refunds
- Retail
- Subscriptions
- Team
- Terminal
- Webhooks
title: Square Order
---
