---
description: ResponseAdditionalDataInstallments schema from Adyen API
layout: schema
name: ResponseAdditionalDataInstallments
properties_list:
- description: Type of installment. The value of `installmentType` should be **IssuerFinanced**.
  name: installmentPaymentData.installmentType
  type: string
- description: Annual interest rate.
  name: installmentPaymentData.option[itemNr].annualPercentageRate
  type: string
- description: First Installment Amount in minor units.
  name: installmentPaymentData.option[itemNr].firstInstallmentAmount
  type: string
- description: Installment fee amount in minor units.
  name: installmentPaymentData.option[itemNr].installmentFee
  type: string
- description: Interest rate for the installment period.
  name: installmentPaymentData.option[itemNr].interestRate
  type: string
- description: Maximum number of installments possible for this payment.
  name: installmentPaymentData.option[itemNr].maximumNumberOfInstallments
  type: string
- description: Minimum number of installments possible for this payment.
  name: installmentPaymentData.option[itemNr].minimumNumberOfInstallments
  type: string
- description: Total number of installments possible for this payment.
  name: installmentPaymentData.option[itemNr].numberOfInstallments
  type: string
- description: Subsequent Installment Amount in minor units.
  name: installmentPaymentData.option[itemNr].subsequentInstallmentAmount
  type: string
- description: Total amount in minor units.
  name: installmentPaymentData.option[itemNr].totalAmountDue
  type: string
- description: 'Possible values: * PayInInstallmentsOnly * PayInFullOnly * PayInFullOrInstallments'
  name: installmentPaymentData.paymentOptions
  type: string
- description: 'The number of installments that the payment amount should be charged with. Example: 5 > Only relevant for card payments in countries that support installments.'
  name: installments.value
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-response-additional-data-installments-schema.json
slug: checkout-response-additional-data-installments
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-response-additional-data-installments-schema.json\",\n  \"title\": \"ResponseAdditionalDataInstallments\",\n  \"description\": \"ResponseAdditionalDataInstallments schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"installmentPaymentData.installmentType\": {\n      \"description\": \"Type of installment. The value of `installmentType` should be **IssuerFinanced**.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].annualPercentageRate\": {\n      \"description\": \"Annual interest rate.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].firstInstallmentAmount\": {\n      \"description\": \"First Installment Amount in minor units.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].installmentFee\"\
  : {\n      \"description\": \"Installment fee amount in minor units.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].interestRate\": {\n      \"description\": \"Interest rate for the installment period.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].maximumNumberOfInstallments\": {\n      \"description\": \"Maximum number of installments possible for this payment.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].minimumNumberOfInstallments\": {\n      \"description\": \"Minimum number of installments possible for this payment.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].numberOfInstallments\": {\n      \"description\": \"Total number of installments possible for this payment.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].subsequentInstallmentAmount\": {\n      \"description\": \"Subsequent Installment Amount\
  \ in minor units.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.option[itemNr].totalAmountDue\": {\n      \"description\": \"Total amount in minor units.\",\n      \"type\": \"string\"\n    },\n    \"installmentPaymentData.paymentOptions\": {\n      \"description\": \"Possible values:\\n* PayInInstallmentsOnly\\n* PayInFullOnly\\n* PayInFullOrInstallments\",\n      \"type\": \"string\"\n    },\n    \"installments.value\": {\n      \"description\": \"The number of installments that the payment amount should be charged with.\\n\\nExample: 5\\n> Only relevant for card payments in countries that support installments.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-response-additional-data-installments-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataInstallments
---
