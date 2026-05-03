---
description: Invoices are statements of amounts owed by a customer, and are either generated one-off, or generated periodically from a subscription.
layout: schema
name: Stripe Invoice
properties_list:
- description: Unique identifier for the object.
  name: id
  type:
  - string
  - 'null'
- description: String representing the object's type.
  name: object
  type: string
- description: The country of the business associated with this invoice.
  name: account_country
  type:
  - string
  - 'null'
- description: The public name of the business associated with this invoice.
  name: account_name
  type:
  - string
  - 'null'
- description: Final amount due at this time for this invoice.
  name: amount_due
  type: integer
- description: The amount, in cents, that was paid.
  name: amount_paid
  type: integer
- description: The difference between amount_due and amount_paid, in cents.
  name: amount_remaining
  type: integer
- description: This is the sum of all the shipping amounts.
  name: amount_shipping
  type: integer
- description: ID of the Connect Application that created the invoice.
  name: application
  type:
  - string
  - 'null'
- description: Number of payment attempts made for this invoice.
  name: attempt_count
  type: integer
- description: Whether an attempt has been made to pay the invoice.
  name: attempted
  type: boolean
- description: Controls whether Stripe performs automatic collection of the invoice.
  name: auto_advance
  type: boolean
- description: Indicates the reason why the invoice was created.
  name: billing_reason
  type:
  - string
  - 'null'
- description: ID of the latest charge generated for this invoice.
  name: charge
  type:
  - string
  - 'null'
- description: How the invoice's collection is handled.
  name: collection_method
  type: string
- description: Time at which the object was created.
  name: created
  type: integer
- description: Three-letter ISO currency code, in lowercase.
  name: currency
  type: string
- description: The ID of the customer who will be billed.
  name: customer
  type:
  - string
  - 'null'
- description: The customer's email.
  name: customer_email
  type:
  - string
  - 'null'
- description: The customer's name.
  name: customer_name
  type:
  - string
  - 'null'
- description: An arbitrary string attached to the object.
  name: description
  type:
  - string
  - 'null'
- description: The date on which payment for this invoice is due.
  name: due_date
  type:
  - integer
  - 'null'
- description: The date when this invoice is in effect.
  name: effective_at
  type:
  - integer
  - 'null'
- description: The URL for the hosted invoice page.
  name: hosted_invoice_url
  type:
  - string
  - 'null'
- description: The link to download the PDF for the invoice.
  name: invoice_pdf
  type:
  - string
  - 'null'
- description: The individual line items that make up the invoice.
  name: lines
  type: object
- description: Has the value true if the object exists in live mode.
  name: livemode
  type: boolean
- description: Set of key-value pairs that you can attach to an object.
  name: metadata
  type:
  - object
  - 'null'
- description: A unique, identifying string that appears on emails sent for this invoice.
  name: number
  type:
  - string
  - 'null'
- description: Whether payment was successfully collected for this invoice.
  name: paid
  type: boolean
- description: Returns true if the invoice was manually marked paid.
  name: paid_out_of_band
  type: boolean
- description: The PaymentIntent associated with this invoice.
  name: payment_intent
  type:
  - string
  - 'null'
- description: End of the usage period during which invoice items were added to this invoice.
  name: period_end
  type: integer
- description: Start of the usage period during which invoice items were added to this invoice.
  name: period_start
  type: integer
- description: The status of the invoice.
  name: status
  type:
  - string
  - 'null'
- description: The subscription that this invoice was prepared for, if any.
  name: subscription
  type:
  - string
  - 'null'
- description: Total of all subscriptions, invoice items, and prorations on the invoice before any invoice level discount or exclusive tax is applied.
  name: subtotal
  type: integer
- description: The amount of tax on this invoice.
  name: tax
  type:
  - integer
  - 'null'
- description: Total after discounts and taxes.
  name: total
  type: integer
- description: The aggregate amounts calculated per discount across all line items.
  name: total_discount_amounts
  type:
  - array
  - 'null'
- description: The integer amount in cents representing the total amount of the invoice including all discounts but excluding all tax.
  name: total_excluding_tax
  type:
  - integer
  - 'null'
- description: The aggregate amounts calculated per tax rate for all line items.
  name: total_tax_amounts
  type: array
- description: Invoices are automatically paid or sent 1 hour after webhooks are delivered.
  name: webhooks_delivered_at
  type:
  - integer
  - 'null'
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-invoice.json
slug: stripe-invoice
source_filename: stripe-invoice.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/invoice\",\n  \"title\": \"Stripe Invoice\",\n  \"description\": \"Invoices are statements of amounts owed by a customer, and are either generated one-off, or generated periodically from a subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^in_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"invoice\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"account_country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The country of the business associated with this invoice.\"\n    },\n    \"account_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The public name of the business associated with this invoice.\"\
  \n    },\n    \"amount_due\": {\n      \"type\": \"integer\",\n      \"description\": \"Final amount due at this time for this invoice.\"\n    },\n    \"amount_paid\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount, in cents, that was paid.\"\n    },\n    \"amount_remaining\": {\n      \"type\": \"integer\",\n      \"description\": \"The difference between amount_due and amount_paid, in cents.\"\n    },\n    \"amount_shipping\": {\n      \"type\": \"integer\",\n      \"description\": \"This is the sum of all the shipping amounts.\"\n    },\n    \"application\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the Connect Application that created the invoice.\"\n    },\n    \"attempt_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of payment attempts made for this invoice.\"\n    },\n    \"attempted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether an attempt has been made to pay the invoice.\"\n\
  \    },\n    \"auto_advance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Controls whether Stripe performs automatic collection of the invoice.\"\n    },\n    \"billing_reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates the reason why the invoice was created.\",\n      \"enum\": [\n        \"automatic_pending_invoice_item_invoice\",\n        \"manual\",\n        \"quote_accept\",\n        \"subscription\",\n        \"subscription_create\",\n        \"subscription_cycle\",\n        \"subscription_threshold\",\n        \"subscription_update\",\n        \"upcoming\",\n        null\n      ]\n    },\n    \"charge\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the latest charge generated for this invoice.\"\n    },\n    \"collection_method\": {\n      \"type\": \"string\",\n      \"description\": \"How the invoice's collection is handled.\",\n      \"enum\": [\"charge_automatically\", \"send_invoice\"]\n    },\n\
  \    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was created.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter ISO currency code, in lowercase.\"\n    },\n    \"customer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the customer who will be billed.\"\n    },\n    \"customer_email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer's email.\"\n    },\n    \"customer_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer's name.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An arbitrary string attached to the object.\"\n    },\n    \"due_date\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The date on which payment for this invoice is due.\"\n    },\n    \"effective_at\": {\n      \"type\": [\"integer\", \"\
  null\"],\n      \"description\": \"The date when this invoice is in effect.\"\n    },\n    \"hosted_invoice_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The URL for the hosted invoice page.\"\n    },\n    \"invoice_pdf\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The link to download the PDF for the invoice.\"\n    },\n    \"lines\": {\n      \"type\": \"object\",\n      \"description\": \"The individual line items that make up the invoice.\"\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode.\"\n    },\n    \"metadata\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Set of key-value pairs that you can attach to an object.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"number\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A unique, identifying string that appears on emails\
  \ sent for this invoice.\"\n    },\n    \"paid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether payment was successfully collected for this invoice.\"\n    },\n    \"paid_out_of_band\": {\n      \"type\": \"boolean\",\n      \"description\": \"Returns true if the invoice was manually marked paid.\"\n    },\n    \"payment_intent\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The PaymentIntent associated with this invoice.\"\n    },\n    \"period_end\": {\n      \"type\": \"integer\",\n      \"description\": \"End of the usage period during which invoice items were added to this invoice.\"\n    },\n    \"period_start\": {\n      \"type\": \"integer\",\n      \"description\": \"Start of the usage period during which invoice items were added to this invoice.\"\n    },\n    \"status\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The status of the invoice.\",\n      \"enum\": [\"draft\", \"open\", \"paid\", \"uncollectible\"\
  , \"void\", null]\n    },\n    \"subscription\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The subscription that this invoice was prepared for, if any.\"\n    },\n    \"subtotal\": {\n      \"type\": \"integer\",\n      \"description\": \"Total of all subscriptions, invoice items, and prorations on the invoice before any invoice level discount or exclusive tax is applied.\"\n    },\n    \"tax\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The amount of tax on this invoice.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total after discounts and taxes.\"\n    },\n    \"total_discount_amounts\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"The aggregate amounts calculated per discount across all line items.\",\n      \"items\": { \"type\": \"object\" }\n    },\n    \"total_excluding_tax\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The integer amount\
  \ in cents representing the total amount of the invoice including all discounts but excluding all tax.\"\n    },\n    \"total_tax_amounts\": {\n      \"type\": \"array\",\n      \"description\": \"The aggregate amounts calculated per tax rate for all line items.\",\n      \"items\": { \"type\": \"object\" }\n    },\n    \"webhooks_delivered_at\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Invoices are automatically paid or sent 1 hour after webhooks are delivered.\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"amount_due\",\n    \"amount_paid\",\n    \"amount_remaining\",\n    \"attempt_count\",\n    \"attempted\",\n    \"collection_method\",\n    \"created\",\n    \"currency\",\n    \"livemode\",\n    \"paid\",\n    \"paid_out_of_band\",\n    \"period_end\",\n    \"period_start\",\n    \"subtotal\",\n    \"total\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-invoice.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Invoice
---
