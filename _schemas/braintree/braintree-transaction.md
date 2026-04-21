---
description: Represents a payment transaction processed through the Braintree gateway. A transaction captures the full lifecycle from authorization through settlement, refund, or void, and supports credit and debit cards, PayPal, Apple Pay, Google Pay, Venmo, ACH, and SEPA payment methods.
layout: schema
name: Braintree Transaction
properties_list:
- description: Unique identifier for the transaction assigned by Braintree.
  name: id
  type: string
- description: The transaction amount as a decimal string in the transaction currency.
  name: amount
  type: string
- description: The current processing status of the transaction.
  name: status
  type: string
- description: The type of transaction. 'sale' represents a charge and 'credit' represents a refund.
  name: type
  type: string
- description: ISO 4217 three-letter currency code for the transaction.
  name: currency_iso_code
  type: string
- description: Merchant-provided order identifier associated with this transaction for reconciliation.
  name: order_id
  type: string
- description: Identifier of the Braintree merchant account used to process this transaction.
  name: merchant_account_id
  type: string
- description: Identifier of the customer in the Braintree Vault associated with this transaction, if applicable.
  name: customer_id
  type: string
- description: Token of the vaulted payment method used for this transaction, if applicable.
  name: payment_method_token
  type: string
- description: The one-time payment method nonce used for this transaction, if applicable.
  name: payment_method_nonce
  type: string
- description: The processor-specific response code returned when the transaction was processed.
  name: processor_response_code
  type: string
- description: Human-readable text description of the processor response code.
  name: processor_response_text
  type: string
- description: The reason the Braintree gateway rejected the transaction, if applicable.
  name: gateway_rejection_reason
  type: string
- description: The tax amount included in the transaction total, as a decimal string.
  name: tax_amount
  type: string
- description: The shipping amount included in the transaction total, as a decimal string.
  name: shipping_amount
  type: string
- description: Indicates the origin of the transaction for network reporting requirements.
  name: transaction_source
  type: string
- description: Billing address associated with this transaction.
  name: billing
  type: object
- description: Shipping address associated with this transaction.
  name: shipping
  type: object
- description: Summary of the customer associated with this transaction.
  name: customer_details
  type: object
- description: Masked credit or debit card details used in this transaction.
  name: credit_card_details
  type: object
- description: Dynamic descriptor fields that appear on the customer's bank statement.
  name: descriptor
  type: object
- description: List of transaction identifiers for refund transactions created against this transaction.
  name: refund_ids
  type: array
- description: For refund transactions, the identifier of the original transaction being refunded.
  name: refunded_transaction_id
  type: string
- description: Identifier of the subscription that generated this transaction, if applicable.
  name: subscription_id
  type: string
- description: Line items for Level 3 processing data, up to 249 items.
  name: line_items
  type: array
- description: Disbursement information for when the transaction funds were or will be sent to the merchant.
  name: disbursement_details
  type: object
- description: Timestamp when the transaction was created, in ISO 8601 format.
  name: created_at
  type: string
- description: Timestamp when the transaction was last updated, in ISO 8601 format.
  name: updated_at
  type: string
provider_name: braintree
provider_slug: braintree
schema_file: json-schema/braintree-transaction-schema.json
slug: braintree-transaction
tags: []
title: Braintree Transaction
---
