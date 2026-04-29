---
description: Represents an Affirm checkout session containing all order details, customer information, and merchant configuration required to initiate the Affirm buy now pay later financing flow. Checkout objects are created via the Checkout API and result in a checkout token that is exchanged for a transaction authorization after customer confirmation.
layout: schema
name: Affirm Checkout
properties_list:
- description: Unique identifier assigned to this checkout session by Affirm.
  name: checkout_id
  type: string
- description: Current status of the checkout session.
  name: checkout_status
  type: string
- description: The checkout flow type used for this session (e.g., classic, direct).
  name: checkout_flow_type
  type: string
- description: ''
  name: merchant
  type: object
- description: ''
  name: shipping
  type: object
- description: ''
  name: billing
  type: object
- description: ''
  name: store
  type: object
- description: Array of item objects representing the products being purchased in this checkout.
  name: items
  type: array
- description: Map of discount codes to discount objects applied to this checkout.
  name: discounts
  type: object
- description: Arbitrary key-value metadata for merchant tracking. All values must be strings.
  name: metadata
  type: object
- description: The merchant's internal order identifier stored for future reference and reconciliation.
  name: order_id
  type: string
- description: Three-letter ISO 4217 currency code in uppercase.
  name: currency
  type: string
- description: A financing program code applied to this checkout that determines the loan terms presented to the customer.
  name: financing_program
  type: string
- description: Internal financing program identifier applied to this checkout.
  name: financial_program_name
  type: string
- description: Customer-facing financing program name.
  name: financial_program_external_name
  type: string
- description: The total shipping amount in cents.
  name: shipping_amount
  type: integer
- description: The total tax amount in cents.
  name: tax_amount
  type: integer
- description: The total amount of the checkout in the smallest currency unit (cents for USD/CAD, pence for GBP).
  name: total
  type: integer
- description: ISO 8601 timestamp specifying when the checkout session expires.
  name: checkout_expiration
  type: string
- description: Time-to-live deadline by which the customer must confirm the checkout.
  name: expiration_time
  type: string
- description: Loan billing frequency for the financing applied to this checkout.
  name: billing_frequency
  type: string
- description: Version of the Affirm API used to create this checkout.
  name: api_version
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/affirm-checkout-schema.json
slug: affirm-checkout
source_filename: affirm-checkout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://affirm.com/schemas/affirm/checkout.json\",\n  \"title\": \"Affirm Checkout\",\n  \"description\": \"Represents an Affirm checkout session containing all order details, customer information, and merchant configuration required to initiate the Affirm buy now pay later financing flow. Checkout objects are created via the Checkout API and result in a checkout token that is exchanged for a transaction authorization after customer confirmation.\",\n  \"type\": \"object\",\n  \"required\": [\"merchant\", \"items\", \"currency\", \"total\"],\n  \"properties\": {\n    \"checkout_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to this checkout session by Affirm.\"\n    },\n    \"checkout_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the checkout session.\",\n      \"enum\": [\"pending\", \"confirmed\", \"failed\", \"\
  expired\"]\n    },\n    \"checkout_flow_type\": {\n      \"type\": \"string\",\n      \"description\": \"The checkout flow type used for this session (e.g., classic, direct).\",\n      \"examples\": [\"classic\", \"direct\"]\n    },\n    \"merchant\": {\n      \"$ref\": \"#/$defs/MerchantObject\"\n    },\n    \"shipping\": {\n      \"$ref\": \"#/$defs/ContactObject\"\n    },\n    \"billing\": {\n      \"$ref\": \"#/$defs/ContactObject\"\n    },\n    \"store\": {\n      \"$ref\": \"#/$defs/StoreObject\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of item objects representing the products being purchased in this checkout.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/ItemObject\"\n      }\n    },\n    \"discounts\": {\n      \"type\": \"object\",\n      \"description\": \"Map of discount codes to discount objects applied to this checkout.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/DiscountObject\"\
  \n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary key-value metadata for merchant tracking. All values must be strings.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's internal order identifier stored for future reference and reconciliation.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ISO 4217 currency code in uppercase.\",\n      \"enum\": [\"USD\", \"CAD\", \"GBP\"]\n    },\n    \"financing_program\": {\n      \"type\": \"string\",\n      \"description\": \"A financing program code applied to this checkout that determines the loan terms presented to the customer.\"\n    },\n    \"financial_program_name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal financing program identifier applied to this checkout.\"\n    },\n    \"financial_program_external_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Customer-facing financing program name.\"\n    },\n    \"shipping_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total shipping amount in cents.\",\n      \"minimum\": 0\n    },\n    \"tax_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total tax amount in cents.\",\n      \"minimum\": 0\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total amount of the checkout in the smallest currency unit (cents for USD/CAD, pence for GBP).\",\n      \"minimum\": 0\n    },\n    \"checkout_expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp specifying when the checkout session expires.\"\n    },\n    \"expiration_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time-to-live deadline by which the customer must confirm the checkout.\"\n \
  \   },\n    \"billing_frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Loan billing frequency for the financing applied to this checkout.\"\n    },\n    \"api_version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the Affirm API used to create this checkout.\"\n    }\n  },\n  \"$defs\": {\n    \"MerchantObject\": {\n      \"type\": \"object\",\n      \"description\": \"Merchant-specific configuration for the checkout session including callback URLs and API credentials.\",\n      \"required\": [\"user_confirmation_url\", \"user_cancel_url\"],\n      \"properties\": {\n        \"public_api_key\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant's public API key. Required for server-side checkout and store endpoint calls.\"\n        },\n        \"user_confirmation_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL the customer is redirected to after successfully\
  \ completing the Affirm checkout flow. The checkout_token is delivered here.\"\n        },\n        \"user_cancel_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL the customer is redirected to if they cancel or abandon the Affirm checkout flow.\"\n        },\n        \"user_confirmation_url_action\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies how the checkout_token is delivered to the user_confirmation_url. POST sends it as a form body field; GET appends it as a query parameter.\",\n          \"enum\": [\"POST\", \"GET\"],\n          \"default\": \"POST\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant's display name shown to customers during the checkout flow.\"\n        }\n      }\n    },\n    \"ContactObject\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for shipping or billing including name, address,\
  \ email, and phone number.\",\n      \"properties\": {\n        \"name\": {\n          \"$ref\": \"#/$defs/NameObject\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/AddressObject\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address for this contact.\"\n        },\n        \"phone_number\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number for this contact in E.164 format.\",\n          \"pattern\": \"^\\\\+?[1-9]\\\\d{1,14}$\"\n        }\n      }\n    },\n    \"NameObject\": {\n      \"type\": \"object\",\n      \"description\": \"A person's name split into first and last name components.\",\n      \"properties\": {\n        \"first\": {\n          \"type\": \"string\",\n          \"description\": \"The person's first name.\",\n          \"maxLength\": 100\n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The person's last name.\",\n          \"maxLength\": 100\n        },\n        \"full\": {\n          \"type\": \"string\",\n          \"description\": \"The person's full name as a single string.\",\n          \"maxLength\": 200\n        }\n      }\n    },\n    \"AddressObject\": {\n      \"type\": \"object\",\n      \"description\": \"A postal address used for shipping or billing.\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\",\n          \"description\": \"Primary street address line.\",\n          \"maxLength\": 200\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line for apartment, suite, or unit number.\",\n          \"maxLength\": 200\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City or locality name.\",\n          \"maxLength\": 100\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"State, province, or region code.\",\n          \"maxLength\": 50\n        },\n        \"zipcode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code.\",\n          \"maxLength\": 20\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 country code.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"ItemObject\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a single line item in the checkout including product details and pricing.\",\n      \"required\": [\"display_name\", \"sku\", \"unit_price\", \"qty\"],\n      \"properties\": {\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"Customer-facing product name displayed during the checkout flow.\",\n          \"maxLength\": 500\n        },\n        \"sku\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant's stock keeping unit\
  \ identifier for this product.\",\n          \"maxLength\": 200\n        },\n        \"unit_price\": {\n          \"type\": \"integer\",\n          \"description\": \"Unit price of the item in the smallest currency unit (e.g., cents).\",\n          \"minimum\": 0\n        },\n        \"qty\": {\n          \"type\": \"integer\",\n          \"description\": \"Quantity of this item included in the order.\",\n          \"minimum\": 1\n        },\n        \"item_image_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the product image displayed to the customer.\"\n        },\n        \"item_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the product page on the merchant's website.\"\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"description\": \"Nested array of category strings representing the product's taxonomy.\",\n          \"items\"\
  : {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"StoreObject\": {\n      \"type\": \"object\",\n      \"description\": \"Address details for in-store transactions where the purchase is made at a physical merchant location.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the store location.\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/AddressObject\"\n        }\n      }\n    },\n    \"DiscountObject\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a discount applied to the checkout with an amount and display name.\",\n      \"properties\": {\n        \"discount_amount\": {\n          \"type\": \"integer\",\n          \"description\": \"The discount amount in cents.\",\n          \"minimum\": 0\n        },\n        \"discount_display_name\": {\n          \"\
  type\": \"string\",\n          \"description\": \"Customer-facing name or description of the discount.\",\n          \"maxLength\": 200\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/affirm-checkout-schema.json
tags: []
title: Affirm Checkout
---
