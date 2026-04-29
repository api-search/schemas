---
description: Represents a subscription purchased by a customer. Subscriptions enable sellers to generate recurring revenue by offering scheduled fulfillment of products or services with configurable billing periods, pricing, and discounts.
layout: schema
name: Square Subscription
properties_list:
- description: The Square-assigned ID of the subscription.
  name: id
  type: string
- description: The ID of the location associated with the subscription.
  name: location_id
  type: string
- description: The ID of the subscribed-to subscription plan variation.
  name: plan_variation_id
  type: string
- description: The ID of the subscribing customer profile.
  name: customer_id
  type: string
- description: The YYYY-MM-DD-formatted date to start the subscription.
  name: start_date
  type: string
- description: The YYYY-MM-DD-formatted date to cancel the subscription, when the subscription status changes to CANCELED and the subscription billing stops.
  name: canceled_date
  type: string
- description: The YYYY-MM-DD-formatted date up to when the subscriber is invoiced for the subscription.
  name: charged_through_date
  type: string
- description: The current status of the subscription.
  name: status
  type: string
- description: 'The tax amount applied when billing the subscription. The percentage is expressed in decimal form, using a ''.'' as the decimal separator and without a ''%'' sign. For example, a value of 7.5 corresponds '
  name: tax_percentage
  type: string
- description: The IDs of the invoices created for the subscription, listed in order when the invoices were created (newest invoices appear first).
  name: invoice_ids
  type: array
- description: A custom price which overrides the cost of a subscription plan variation with STATIC pricing.
  name: price_override_money
  type: object
- description: The version of the object. When updating an object, the version supplied must match the version in the database.
  name: version
  type: integer
- description: The timestamp when the subscription was created, in RFC 3339 format.
  name: created_at
  type: string
- description: The ID of the subscriber's card used to charge for the subscription.
  name: card_id
  type: string
- description: 'Timezone that will be used in date calculations for the subscription. Defaults to the timezone of the location based on location_id. Format: the IANA Timezone Database identifier.'
  name: timezone
  type: string
- description: The origination details of the subscription.
  name: source
  type: object
- description: The list of scheduled actions on this subscription.
  name: actions
  type: array
- description: The day of the month on which the subscription will issue invoices and publish orders.
  name: monthly_billing_anchor_date
  type: integer
- description: The subscription phases that define the billing schedule.
  name: phases
  type: array
provider_name: Square
provider_slug: square
schema_file: json-schema/subscription.json
slug: subscription
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/square/blob/main/json-schema/subscription.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Square Subscription\",\n  \"description\": \"Represents a subscription purchased by a customer. Subscriptions enable sellers to generate recurring revenue by offering scheduled fulfillment of products or services with configurable billing periods, pricing, and discounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Square-assigned ID of the subscription.\",\n      \"maxLength\": 255,\n      \"readOnly\": true\n    },\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the location associated with the subscription.\",\n      \"readOnly\": true\n    },\n    \"plan_variation_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subscribed-to subscription plan variation.\"\
  ,\n      \"readOnly\": true\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subscribing customer profile.\",\n      \"readOnly\": true\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The YYYY-MM-DD-formatted date to start the subscription.\",\n      \"readOnly\": true\n    },\n    \"canceled_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The YYYY-MM-DD-formatted date to cancel the subscription, when the subscription status changes to CANCELED and the subscription billing stops.\"\n    },\n    \"charged_through_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The YYYY-MM-DD-formatted date up to when the subscriber is invoiced for the subscription.\",\n      \"readOnly\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of\
  \ the subscription.\",\n      \"enum\": [\"PENDING\", \"ACTIVE\", \"CANCELED\", \"DEACTIVATED\", \"PAUSED\"],\n      \"readOnly\": true\n    },\n    \"tax_percentage\": {\n      \"type\": \"string\",\n      \"description\": \"The tax amount applied when billing the subscription. The percentage is expressed in decimal form, using a '.' as the decimal separator and without a '%' sign. For example, a value of 7.5 corresponds to 7.5%.\"\n    },\n    \"invoice_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The IDs of the invoices created for the subscription, listed in order when the invoices were created (newest invoices appear first).\",\n      \"readOnly\": true\n    },\n    \"price_override_money\": {\n      \"$ref\": \"money.json\",\n      \"description\": \"A custom price which overrides the cost of a subscription plan variation with STATIC pricing.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n\
  \      \"format\": \"int64\",\n      \"description\": \"The version of the object. When updating an object, the version supplied must match the version in the database.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the subscription was created, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"card_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the subscriber's card used to charge for the subscription.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone that will be used in date calculations for the subscription. Defaults to the timezone of the location based on location_id. Format: the IANA Timezone Database identifier.\",\n      \"readOnly\": true\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The origination details of the subscription.\",\n      \"properties\": {\n       \
  \ \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name used to identify the place that created the subscription.\"\n        }\n      }\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the scheduled action.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of the action.\",\n            \"enum\": [\"CANCEL\", \"PAUSE\", \"RESUME\", \"SWAP_PLAN\", \"CHANGE_BILLING_ANCHOR_DATE\"]\n          },\n          \"effective_date\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"description\": \"The YYYY-MM-DD-formatted date when the action will take effect.\"\n          }\n        }\n      },\n      \"description\": \"The list of scheduled actions on this subscription.\"\n    },\n  \
  \  \"monthly_billing_anchor_date\": {\n      \"type\": \"integer\",\n      \"description\": \"The day of the month on which the subscription will issue invoices and publish orders.\",\n      \"minimum\": 1,\n      \"maximum\": 31\n    },\n    \"phases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uid\": {\n            \"type\": \"string\",\n            \"description\": \"The Square-assigned ID of the subscription phase.\"\n          },\n          \"cadence\": {\n            \"type\": \"string\",\n            \"description\": \"The billing cadence of the phase.\",\n            \"enum\": [\"DAILY\", \"WEEKLY\", \"EVERY_TWO_WEEKS\", \"THIRTY_DAYS\", \"SIXTY_DAYS\", \"NINETY_DAYS\", \"MONTHLY\", \"EVERY_TWO_MONTHS\", \"QUARTERLY\", \"EVERY_FOUR_MONTHS\", \"EVERY_SIX_MONTHS\", \"ANNUAL\", \"EVERY_TWO_YEARS\"]\n          },\n          \"periods\": {\n            \"type\": \"integer\",\n            \"description\":\
  \ \"The number of periods the phase lasts.\"\n          },\n          \"recurring_price_money\": {\n            \"$ref\": \"money.json\",\n            \"description\": \"The amount billed per period during this phase.\"\n          },\n          \"ordinal\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The position this phase appears in the sequence of phases.\"\n          }\n        }\n      },\n      \"description\": \"The subscription phases that define the billing schedule.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/square/refs/heads/main/json-schema/subscription.json
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
title: Square Subscription
---
