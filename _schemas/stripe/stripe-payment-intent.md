---
description: A PaymentIntent guides you through the process of collecting a payment from your customer. It tracks charge attempts and payment state changes throughout the process.
layout: schema
name: Stripe Payment Intent
properties_list:
- description: Unique identifier for the object.
  name: id
  type: string
- description: String representing the object's type.
  name: object
  type: string
- description: Amount intended to be collected by this PaymentIntent. A positive integer representing how much to charge in the smallest currency unit.
  name: amount
  type: integer
- description: Amount that can be captured from this PaymentIntent.
  name: amount_capturable
  type: integer
- description: Amount that this PaymentIntent collected.
  name: amount_received
  type: integer
- description: ID of the Connect application that created the PaymentIntent.
  name: application
  type:
  - string
  - 'null'
- description: The amount of the application fee for the resulting payment.
  name: application_fee_amount
  type:
  - integer
  - 'null'
- description: Settings to configure compatible payment methods from the Stripe Dashboard.
  name: automatic_payment_methods
  type:
  - object
  - 'null'
- description: Populated when status is canceled, this is the time at which the PaymentIntent was canceled.
  name: canceled_at
  type:
  - integer
  - 'null'
- description: Reason for cancellation of this PaymentIntent.
  name: cancellation_reason
  type:
  - string
  - 'null'
- description: Controls when the funds are captured from the customer's account.
  name: capture_method
  type: string
- description: The client secret of this PaymentIntent.
  name: client_secret
  type:
  - string
  - 'null'
- description: Describes whether we can confirm this PaymentIntent automatically or if it requires customer action.
  name: confirmation_method
  type: string
- description: Time at which the object was created. Measured in seconds since the Unix epoch.
  name: created
  type: integer
- description: Three-letter ISO currency code, in lowercase.
  name: currency
  type: string
- description: ID of the Customer this PaymentIntent belongs to.
  name: customer
  type:
  - string
  - 'null'
- description: An arbitrary string attached to the object.
  name: description
  type:
  - string
  - 'null'
- description: ID of the invoice that created this PaymentIntent, if it exists.
  name: invoice
  type:
  - string
  - 'null'
- description: The payment error encountered in the previous PaymentIntent confirmation.
  name: last_payment_error
  type:
  - object
  - 'null'
- description: The latest charge created by this PaymentIntent.
  name: latest_charge
  type:
  - string
  - 'null'
- description: Has the value true if the object exists in live mode.
  name: livemode
  type: boolean
- description: Set of key-value pairs that you can attach to an object.
  name: metadata
  type: object
- description: If present, this property tells you what actions you need to take in order for your customer to fulfill a payment.
  name: next_action
  type:
  - object
  - 'null'
- description: The account (if any) for which the funds of the PaymentIntent are intended.
  name: on_behalf_of
  type:
  - string
  - 'null'
- description: ID of the payment method used in this PaymentIntent.
  name: payment_method
  type:
  - string
  - 'null'
- description: Payment-method-specific configuration for this PaymentIntent.
  name: payment_method_options
  type:
  - object
  - 'null'
- description: The list of payment method types that this PaymentIntent is allowed to use.
  name: payment_method_types
  type: array
- description: If present, this property tells you about the processing state of the payment.
  name: processing
  type:
  - object
  - 'null'
- description: Email address that the receipt for the resulting payment will be sent to.
  name: receipt_email
  type:
  - string
  - 'null'
- description: ID of the review associated with this PaymentIntent, if any.
  name: review
  type:
  - string
  - 'null'
- description: Indicates that you intend to make future payments with this PaymentIntent's payment method.
  name: setup_future_usage
  type:
  - string
  - 'null'
- description: Shipping information for this PaymentIntent.
  name: shipping
  type:
  - object
  - 'null'
- description: For card charges, use statement_descriptor_suffix. Otherwise, you can use this value as the complete description of a charge on your customers' statements.
  name: statement_descriptor
  type:
  - string
  - 'null'
- description: Provides information about a card payment that customers see on their statements.
  name: statement_descriptor_suffix
  type:
  - string
  - 'null'
- description: Status of this PaymentIntent.
  name: status
  type: string
- description: The data that automatically creates a Transfer after the payment finalizes.
  name: transfer_data
  type:
  - object
  - 'null'
- description: A string that identifies the resulting payment as part of a group.
  name: transfer_group
  type:
  - string
  - 'null'
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-payment-intent.json
slug: stripe-payment-intent
source_filename: stripe-payment-intent.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/payment-intent\",\n  \"title\": \"Stripe Payment Intent\",\n  \"description\": \"A PaymentIntent guides you through the process of collecting a payment from your customer. It tracks charge attempts and payment state changes throughout the process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^pi_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"payment_intent\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount intended to be collected by this PaymentIntent. A positive integer representing how much to charge in the smallest currency unit.\"\n    },\n    \"amount_capturable\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Amount that can be captured from this PaymentIntent.\"\n    },\n    \"amount_received\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount that this PaymentIntent collected.\"\n    },\n    \"application\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the Connect application that created the PaymentIntent.\"\n    },\n    \"application_fee_amount\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The amount of the application fee for the resulting payment.\"\n    },\n    \"automatic_payment_methods\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Settings to configure compatible payment methods from the Stripe Dashboard.\",\n      \"properties\": {\n        \"allow_redirects\": {\n          \"type\": \"string\",\n          \"enum\": [\"always\", \"never\"]\n        },\n        \"enabled\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"canceled_at\"\
  : {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Populated when status is canceled, this is the time at which the PaymentIntent was canceled.\"\n    },\n    \"cancellation_reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reason for cancellation of this PaymentIntent.\",\n      \"enum\": [\"abandoned\", \"automatic\", \"duplicate\", \"failed_invoice\", \"fraudulent\", \"requested_by_customer\", \"void_invoice\", null]\n    },\n    \"capture_method\": {\n      \"type\": \"string\",\n      \"description\": \"Controls when the funds are captured from the customer's account.\",\n      \"enum\": [\"automatic\", \"automatic_async\", \"manual\"]\n    },\n    \"client_secret\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The client secret of this PaymentIntent.\"\n    },\n    \"confirmation_method\": {\n      \"type\": \"string\",\n      \"description\": \"Describes whether we can confirm this PaymentIntent automatically\
  \ or if it requires customer action.\",\n      \"enum\": [\"automatic\", \"manual\"]\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was created. Measured in seconds since the Unix epoch.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ISO currency code, in lowercase.\"\n    },\n    \"customer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the Customer this PaymentIntent belongs to.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An arbitrary string attached to the object.\"\n    },\n    \"invoice\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the invoice that created this PaymentIntent, if it exists.\"\n    },\n    \"last_payment_error\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The payment error encountered in the previous PaymentIntent\
  \ confirmation.\",\n      \"properties\": {\n        \"charge\": { \"type\": [\"string\", \"null\"] },\n        \"code\": { \"type\": [\"string\", \"null\"] },\n        \"decline_code\": { \"type\": [\"string\", \"null\"] },\n        \"doc_url\": { \"type\": [\"string\", \"null\"] },\n        \"message\": { \"type\": [\"string\", \"null\"] },\n        \"param\": { \"type\": [\"string\", \"null\"] },\n        \"payment_method\": { \"type\": [\"object\", \"null\"] },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"api_error\", \"card_error\", \"idempotency_error\", \"invalid_request_error\"]\n        }\n      }\n    },\n    \"latest_charge\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The latest charge created by this PaymentIntent.\"\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Set of key-value pairs that you can attach to an object.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"next_action\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"If present, this property tells you what actions you need to take in order for your customer to fulfill a payment.\"\n    },\n    \"on_behalf_of\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The account (if any) for which the funds of the PaymentIntent are intended.\"\n    },\n    \"payment_method\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the payment method used in this PaymentIntent.\"\n    },\n    \"payment_method_options\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Payment-method-specific configuration for this PaymentIntent.\"\n    },\n    \"payment_method_types\": {\n      \"type\": \"array\",\n      \"description\": \"The list of payment\
  \ method types that this PaymentIntent is allowed to use.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"processing\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"If present, this property tells you about the processing state of the payment.\"\n    },\n    \"receipt_email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Email address that the receipt for the resulting payment will be sent to.\"\n    },\n    \"review\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the review associated with this PaymentIntent, if any.\"\n    },\n    \"setup_future_usage\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates that you intend to make future payments with this PaymentIntent's payment method.\",\n      \"enum\": [\"off_session\", \"on_session\", null]\n    },\n    \"shipping\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Shipping information\
  \ for this PaymentIntent.\"\n    },\n    \"statement_descriptor\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For card charges, use statement_descriptor_suffix. Otherwise, you can use this value as the complete description of a charge on your customers' statements.\"\n    },\n    \"statement_descriptor_suffix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provides information about a card payment that customers see on their statements.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of this PaymentIntent.\",\n      \"enum\": [\n        \"canceled\",\n        \"processing\",\n        \"requires_action\",\n        \"requires_capture\",\n        \"requires_confirmation\",\n        \"requires_payment_method\",\n        \"succeeded\"\n      ]\n    },\n    \"transfer_data\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The data that automatically creates a Transfer after the\
  \ payment finalizes.\"\n    },\n    \"transfer_group\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A string that identifies the resulting payment as part of a group.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"object\",\n    \"amount\",\n    \"capture_method\",\n    \"confirmation_method\",\n    \"created\",\n    \"currency\",\n    \"livemode\",\n    \"metadata\",\n    \"payment_method_types\",\n    \"status\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-payment-intent.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Payment Intent
---
