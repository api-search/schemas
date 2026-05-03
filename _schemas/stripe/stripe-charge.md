---
description: The Charge object represents a single attempt to move money into your Stripe account. PaymentIntent confirmation is the most common way to create Charges.
layout: schema
name: Stripe Charge
properties_list:
- description: Unique identifier for the object.
  name: id
  type: string
- description: String representing the object's type.
  name: object
  type: string
- description: Amount intended to be collected by this payment. A positive integer representing how much to charge in the smallest currency unit.
  name: amount
  type: integer
- description: Amount in cents captured.
  name: amount_captured
  type: integer
- description: Amount in cents refunded.
  name: amount_refunded
  type: integer
- description: ID of the Connect application that created the charge.
  name: application
  type:
  - string
  - 'null'
- description: The application fee (if any) for the charge.
  name: application_fee
  type:
  - string
  - 'null'
- description: The amount of the application fee (if any) requested for the charge.
  name: application_fee_amount
  type:
  - integer
  - 'null'
- description: ID of the balance transaction that describes the impact of this charge on your account balance.
  name: balance_transaction
  type:
  - string
  - 'null'
- description: Billing information associated with the payment method at the time of the transaction.
  name: billing_details
  type: object
- description: The full statement descriptor that is passed to card networks.
  name: calculated_statement_descriptor
  type:
  - string
  - 'null'
- description: If the charge was created without capturing, this Boolean represents whether it is still uncaptured or has since been captured.
  name: captured
  type: boolean
- description: Time at which the object was created.
  name: created
  type: integer
- description: Three-letter ISO currency code, in lowercase.
  name: currency
  type: string
- description: ID of the customer this charge is for if one exists.
  name: customer
  type:
  - string
  - 'null'
- description: An arbitrary string attached to the object.
  name: description
  type:
  - string
  - 'null'
- description: Whether the charge has been disputed.
  name: disputed
  type: boolean
- description: ID of the balance transaction that describes the reversal of the balance on your account due to payment failure.
  name: failure_balance_transaction
  type:
  - string
  - 'null'
- description: Error code explaining reason for charge failure.
  name: failure_code
  type:
  - string
  - 'null'
- description: Message to user further explaining reason for charge failure.
  name: failure_message
  type:
  - string
  - 'null'
- description: Information on fraud assessments for the charge.
  name: fraud_details
  type:
  - object
  - 'null'
- description: ID of the invoice this charge is for if one exists.
  name: invoice
  type:
  - string
  - 'null'
- description: Has the value true if the object exists in live mode.
  name: livemode
  type: boolean
- description: Set of key-value pairs that you can attach to an object.
  name: metadata
  type: object
- description: The account (if any) the charge was made on behalf of.
  name: on_behalf_of
  type:
  - string
  - 'null'
- description: Details about whether the payment was accepted and why.
  name: outcome
  type:
  - object
  - 'null'
- description: true if the charge succeeded, or was successfully authorized for later capture.
  name: paid
  type: boolean
- description: ID of the PaymentIntent associated with this charge, if one exists.
  name: payment_intent
  type:
  - string
  - 'null'
- description: ID of the payment method used in this charge.
  name: payment_method
  type:
  - string
  - 'null'
- description: Details about the payment method at the time of the transaction.
  name: payment_method_details
  type:
  - object
  - 'null'
- description: This is the email address that the receipt for this charge was sent to.
  name: receipt_email
  type:
  - string
  - 'null'
- description: This is the transaction number that appears on email receipts sent for this charge.
  name: receipt_number
  type:
  - string
  - 'null'
- description: This is the URL to view the receipt for this charge.
  name: receipt_url
  type:
  - string
  - 'null'
- description: Whether the charge has been fully refunded.
  name: refunded
  type: boolean
- description: A list of refunds that have been applied to the charge.
  name: refunds
  type: object
- description: ID of the review associated with this charge if one exists.
  name: review
  type:
  - string
  - 'null'
- description: Shipping information for the charge.
  name: shipping
  type:
  - object
  - 'null'
- description: This is a legacy field that will be removed in the future.
  name: source
  type:
  - object
  - 'null'
- description: The transfer ID which created this charge.
  name: source_transfer
  type:
  - string
  - 'null'
- description: For card charges, use statement_descriptor_suffix.
  name: statement_descriptor
  type:
  - string
  - 'null'
- description: Provides information about the charge that customers see on their statements.
  name: statement_descriptor_suffix
  type:
  - string
  - 'null'
- description: The status of the payment.
  name: status
  type: string
- description: An optional dictionary including the account to automatically transfer to as part of a destination charge.
  name: transfer_data
  type:
  - object
  - 'null'
- description: A string that identifies this transaction as part of a group.
  name: transfer_group
  type:
  - string
  - 'null'
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-charge.json
slug: stripe-charge
source_filename: stripe-charge.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/charge\",\n  \"title\": \"Stripe Charge\",\n  \"description\": \"The Charge object represents a single attempt to move money into your Stripe account. PaymentIntent confirmation is the most common way to create Charges.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^ch_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"charge\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount intended to be collected by this payment. A positive integer representing how much to charge in the smallest currency unit.\"\n    },\n    \"amount_captured\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount in cents\
  \ captured.\"\n    },\n    \"amount_refunded\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount in cents refunded.\"\n    },\n    \"application\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the Connect application that created the charge.\"\n    },\n    \"application_fee\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The application fee (if any) for the charge.\"\n    },\n    \"application_fee_amount\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The amount of the application fee (if any) requested for the charge.\"\n    },\n    \"balance_transaction\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the balance transaction that describes the impact of this charge on your account balance.\"\n    },\n    \"billing_details\": {\n      \"type\": \"object\",\n      \"description\": \"Billing information associated with the payment method at the time of the transaction.\"\
  ,\n      \"properties\": {\n        \"address\": {\n          \"type\": [\"object\", \"null\"],\n          \"properties\": {\n            \"city\": { \"type\": [\"string\", \"null\"] },\n            \"country\": { \"type\": [\"string\", \"null\"] },\n            \"line1\": { \"type\": [\"string\", \"null\"] },\n            \"line2\": { \"type\": [\"string\", \"null\"] },\n            \"postal_code\": { \"type\": [\"string\", \"null\"] },\n            \"state\": { \"type\": [\"string\", \"null\"] }\n          }\n        },\n        \"email\": { \"type\": [\"string\", \"null\"] },\n        \"name\": { \"type\": [\"string\", \"null\"] },\n        \"phone\": { \"type\": [\"string\", \"null\"] }\n      }\n    },\n    \"calculated_statement_descriptor\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The full statement descriptor that is passed to card networks.\"\n    },\n    \"captured\": {\n      \"type\": \"boolean\",\n      \"description\": \"If the charge was created\
  \ without capturing, this Boolean represents whether it is still uncaptured or has since been captured.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was created.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ISO currency code, in lowercase.\"\n    },\n    \"customer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the customer this charge is for if one exists.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An arbitrary string attached to the object.\"\n    },\n    \"disputed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the charge has been disputed.\"\n    },\n    \"failure_balance_transaction\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the balance transaction that describes the reversal of the balance on your account due to payment\
  \ failure.\"\n    },\n    \"failure_code\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Error code explaining reason for charge failure.\"\n    },\n    \"failure_message\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Message to user further explaining reason for charge failure.\"\n    },\n    \"fraud_details\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Information on fraud assessments for the charge.\"\n    },\n    \"invoice\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the invoice this charge is for if one exists.\"\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Set of key-value pairs that you can attach to an object.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"on_behalf_of\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The account (if any) the charge was made on behalf of.\"\n    },\n    \"outcome\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Details about whether the payment was accepted and why.\",\n      \"properties\": {\n        \"network_status\": { \"type\": [\"string\", \"null\"] },\n        \"reason\": { \"type\": [\"string\", \"null\"] },\n        \"risk_level\": { \"type\": [\"string\", \"null\"] },\n        \"risk_score\": { \"type\": [\"integer\", \"null\"] },\n        \"rule\": { \"type\": [\"string\", \"object\", \"null\"] },\n        \"seller_message\": { \"type\": [\"string\", \"null\"] },\n        \"type\": { \"type\": \"string\" }\n      }\n    },\n    \"paid\": {\n      \"type\": \"boolean\",\n      \"description\": \"true if the charge succeeded, or was successfully authorized for later capture.\"\n    },\n    \"payment_intent\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"ID of the PaymentIntent associated with this charge, if one exists.\"\n    },\n    \"payment_method\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the payment method used in this charge.\"\n    },\n    \"payment_method_details\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Details about the payment method at the time of the transaction.\"\n    },\n    \"receipt_email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"This is the email address that the receipt for this charge was sent to.\"\n    },\n    \"receipt_number\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"This is the transaction number that appears on email receipts sent for this charge.\"\n    },\n    \"receipt_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"This is the URL to view the receipt for this charge.\"\n    },\n    \"refunded\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the charge has been fully refunded.\"\n    },\n    \"refunds\": {\n      \"type\": \"object\",\n      \"description\": \"A list of refunds that have been applied to the charge.\"\n    },\n    \"review\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the review associated with this charge if one exists.\"\n    },\n    \"shipping\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Shipping information for the charge.\"\n    },\n    \"source\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"This is a legacy field that will be removed in the future.\"\n    },\n    \"source_transfer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The transfer ID which created this charge.\"\n    },\n    \"statement_descriptor\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For card charges, use statement_descriptor_suffix.\"\n    },\n    \"statement_descriptor_suffix\": {\n    \
  \  \"type\": [\"string\", \"null\"],\n      \"description\": \"Provides information about the charge that customers see on their statements.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the payment.\",\n      \"enum\": [\"failed\", \"pending\", \"succeeded\"]\n    },\n    \"transfer_data\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"An optional dictionary including the account to automatically transfer to as part of a destination charge.\"\n    },\n    \"transfer_group\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A string that identifies this transaction as part of a group.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"object\",\n    \"amount\",\n    \"amount_captured\",\n    \"amount_refunded\",\n    \"billing_details\",\n    \"captured\",\n    \"created\",\n    \"currency\",\n    \"disputed\",\n    \"livemode\",\n    \"metadata\",\n    \"paid\",\n    \"refunded\",\n    \"\
  status\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-charge.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Charge
---
