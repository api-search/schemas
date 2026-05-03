---
description: Schema for a subscription entity within the SAP BRIM (Billing and Revenue Innovation Management) suite. Represents a customer's subscription to a service or product with full lifecycle, billing, and pricing details.
layout: schema
name: SAP BRIM Subscription
properties_list:
- description: Unique identifier for the subscription
  name: subscriptionId
  type: string
- description: Unique identifier of the customer who owns the subscription
  name: customerId
  type: string
- description: Display name of the customer
  name: customerName
  type: string
- description: Identifier of the subscription plan
  name: planId
  type: string
- description: Display name of the subscription plan
  name: planName
  type: string
- description: Current lifecycle status of the subscription
  name: status
  type: string
- description: How often the subscription is billed
  name: billingFrequency
  type: string
- description: Date when the subscription became or becomes active
  name: startDate
  type: string
- description: Date when the subscription ends (null for open-ended subscriptions)
  name: endDate
  type:
  - string
  - 'null'
- description: End date for the trial period, if applicable
  name: trialEndDate
  type:
  - string
  - 'null'
- description: Start date of the current billing period
  name: currentPeriodStart
  type: string
- description: End date of the current billing period
  name: currentPeriodEnd
  type: string
- description: Date of the next scheduled billing event
  name: nextBillingDate
  type:
  - string
  - 'null'
- description: Whether the subscription automatically renews at the end of each term
  name: autoRenew
  type: boolean
- description: Number of times this subscription has been renewed
  name: renewalCount
  type: integer
- description: Minimum contract term in months
  name: contractTermMonths
  type:
  - integer
  - 'null'
- description: Date when the subscription was or will be cancelled
  name: cancellationDate
  type:
  - string
  - 'null'
- description: Reason provided for cancellation
  name: cancellationReason
  type:
  - string
  - 'null'
- description: The recurring charge amount per billing period
  name: recurringCharge
  type: object
- description: One-time setup fee charged at subscription creation
  name: setupFee
  type: object
- description: Line items included in the subscription
  name: items
  type: array
- description: Discounts applied to this subscription
  name: discounts
  type: array
- description: Identifier of the payment method on file
  name: paymentMethod
  type:
  - string
  - 'null'
- description: Billing address for the subscription
  name: billingAddress
  type: object
- description: Custom key-value metadata associated with the subscription
  name: metadata
  type: object
- description: Timestamp when the subscription was created
  name: createdAt
  type: string
- description: Timestamp when the subscription was last modified
  name: modifiedAt
  type: string
- description: Identifier of the user or system that created the subscription
  name: createdBy
  type: string
- description: Identifier of the user or system that last modified the subscription
  name: modifiedBy
  type: string
provider_name: SAP BRIM (Billing and Revenue Innovation Management)
provider_slug: sap-brim-billing-and-revenue-innovation-management
schema_file: json-schema/sap-brim-subscription-schema.json
slug: sap-brim-subscription
source_filename: sap-brim-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/json-schema/sap-brim-subscription-schema.json\",\n  \"title\": \"SAP BRIM Subscription\",\n  \"description\": \"Schema for a subscription entity within the SAP BRIM (Billing and Revenue Innovation Management) suite. Represents a customer's subscription to a service or product with full lifecycle, billing, and pricing details.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"subscriptionId\",\n    \"customerId\",\n    \"planId\",\n    \"status\",\n    \"startDate\",\n    \"billingFrequency\"\n  ],\n  \"properties\": {\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the subscription\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the customer who owns the subscription\"\
  \n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the customer\"\n    },\n    \"planId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the subscription plan\"\n    },\n    \"planName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the subscription plan\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"SUSPENDED\",\n        \"CANCELLED\",\n        \"EXPIRED\",\n        \"PENDING\",\n        \"TRIAL\"\n      ],\n      \"description\": \"Current lifecycle status of the subscription\"\n    },\n    \"billingFrequency\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MONTHLY\",\n        \"QUARTERLY\",\n        \"SEMI_ANNUAL\",\n        \"ANNUAL\",\n        \"CUSTOM\"\n      ],\n      \"description\": \"How often the subscription is billed\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date\",\n      \"description\": \"Date when the subscription became or becomes active\"\n    },\n    \"endDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date when the subscription ends (null for open-ended subscriptions)\"\n    },\n    \"trialEndDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"End date for the trial period, if applicable\"\n    },\n    \"currentPeriodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the current billing period\"\n    },\n    \"currentPeriodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the current billing period\"\n    },\n    \"nextBillingDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date of the next scheduled billing event\"\n    },\n    \"autoRenew\": {\n   \
  \   \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether the subscription automatically renews at the end of each term\"\n    },\n    \"renewalCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of times this subscription has been renewed\"\n    },\n    \"contractTermMonths\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 1,\n      \"description\": \"Minimum contract term in months\"\n    },\n    \"cancellationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date when the subscription was or will be cancelled\"\n    },\n    \"cancellationReason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reason provided for cancellation\"\n    },\n    \"recurringCharge\": {\n      \"$ref\": \"#/$defs/monetaryAmount\",\n      \"description\": \"The recurring charge amount per billing period\"\n    },\n    \"setupFee\": {\n     \
  \ \"$ref\": \"#/$defs/monetaryAmount\",\n      \"description\": \"One-time setup fee charged at subscription creation\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Line items included in the subscription\",\n      \"items\": {\n        \"$ref\": \"#/$defs/subscriptionItem\"\n      }\n    },\n    \"discounts\": {\n      \"type\": \"array\",\n      \"description\": \"Discounts applied to this subscription\",\n      \"items\": {\n        \"$ref\": \"#/$defs/discount\"\n      }\n    },\n    \"paymentMethod\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Identifier of the payment method on file\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/$defs/address\",\n      \"description\": \"Billing address for the subscription\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom key-value metadata associated with the\
  \ subscription\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the subscription was created\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the subscription was last modified\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user or system that created the subscription\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user or system that last modified the subscription\"\n    }\n  },\n  \"$defs\": {\n    \"monetaryAmount\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"value\",\n        \"currency\"\n      ],\n      \"properties\": {\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"The monetary value\"\n        },\n        \"currency\": {\n         \
  \ \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 currency code\"\n        }\n      }\n    },\n    \"subscriptionItem\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"itemId\",\n        \"productId\",\n        \"quantity\"\n      ],\n      \"properties\": {\n        \"itemId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the subscription item\"\n        },\n        \"productId\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the product or service\"\n        },\n        \"productName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the product or service\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the line item\"\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\"\
  : \"Quantity of the item\"\n        },\n        \"unitPrice\": {\n          \"$ref\": \"#/$defs/monetaryAmount\",\n          \"description\": \"Price per unit\"\n        },\n        \"totalPrice\": {\n          \"$ref\": \"#/$defs/monetaryAmount\",\n          \"description\": \"Total price for the item (quantity x unitPrice)\"\n        },\n        \"billingType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"RECURRING\",\n            \"ONE_TIME\",\n            \"USAGE_BASED\"\n          ],\n          \"description\": \"How this item is billed\"\n        },\n        \"includedUnits\": {\n          \"type\": [\"integer\", \"null\"],\n          \"minimum\": 0,\n          \"description\": \"Number of units included in the base price for usage-based items\"\n        },\n        \"overageRate\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Rate per unit above the included quantity\"\n        },\n        \"metadata\": {\n          \"\
  type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"discount\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"discountId\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"discountId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the discount\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the discount\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"PERCENTAGE\",\n            \"FIXED_AMOUNT\",\n            \"FREE_TRIAL\"\n          ],\n          \"description\": \"Type of discount\"\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"Discount value (percentage or fixed amount)\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n      \
  \    \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"Currency for fixed-amount discounts\"\n        },\n        \"couponCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Coupon code that applied this discount\"\n        },\n        \"validFrom\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Start date of discount validity\"\n        },\n        \"validTo\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"End date of discount validity\"\n        }\n      }\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"line2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n     \
  \     \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-brim-billing-and-revenue-innovation-management/refs/heads/main/json-schema/sap-brim-subscription-schema.json
tags:
- Billing
- Enterprise
- Order to Cash
- Revenue Management
- SAP
- Subscription Management
- Usage-Based Pricing
title: SAP BRIM Subscription
---
