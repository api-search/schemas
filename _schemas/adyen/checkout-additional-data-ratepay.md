---
description: AdditionalDataRatepay schema from Adyen API
layout: schema
name: AdditionalDataRatepay
properties_list:
- description: Amount the customer has to pay each month.
  name: ratepay.installmentAmount
  type: string
- description: Interest rate of this installment.
  name: ratepay.interestRate
  type: string
- description: Amount of the last installment.
  name: ratepay.lastInstallmentAmount
  type: string
- description: Calendar day of the first payment.
  name: ratepay.paymentFirstday
  type: string
- description: Date the merchant delivered the goods to the customer.
  name: ratepaydata.deliveryDate
  type: string
- description: Date by which the customer must settle the payment.
  name: ratepaydata.dueDate
  type: string
- description: Invoice date, defined by the merchant. If not included, the invoice date is set to the delivery date.
  name: ratepaydata.invoiceDate
  type: string
- description: Identification name or number for the invoice, defined by the merchant.
  name: ratepaydata.invoiceId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-ratepay-schema.json
slug: checkout-additional-data-ratepay
source_filename: checkout-additional-data-ratepay-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-ratepay-schema.json\",\n  \"title\": \"AdditionalDataRatepay\",\n  \"description\": \"AdditionalDataRatepay schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ratepay.installmentAmount\": {\n      \"description\": \"Amount the customer has to pay each month.\",\n      \"type\": \"string\"\n    },\n    \"ratepay.interestRate\": {\n      \"description\": \"Interest rate of this installment.\",\n      \"type\": \"string\"\n    },\n    \"ratepay.lastInstallmentAmount\": {\n      \"description\": \"Amount of the last installment.\",\n      \"type\": \"string\"\n    },\n    \"ratepay.paymentFirstday\": {\n      \"description\": \"Calendar day of the first payment.\",\n      \"type\": \"string\"\n    },\n    \"ratepaydata.deliveryDate\": {\n      \"description\": \"Date\
  \ the merchant delivered the goods to the customer.\",\n      \"type\": \"string\"\n    },\n    \"ratepaydata.dueDate\": {\n      \"description\": \"Date by which the customer must settle the payment.\",\n      \"type\": \"string\"\n    },\n    \"ratepaydata.invoiceDate\": {\n      \"description\": \"Invoice date, defined by the merchant. If not included, the invoice date is set to the delivery date.\",\n      \"type\": \"string\"\n    },\n    \"ratepaydata.invoiceId\": {\n      \"description\": \"Identification name or number for the invoice, defined by the merchant.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-ratepay-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataRatepay
---
