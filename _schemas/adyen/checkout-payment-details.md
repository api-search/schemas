---
description: PaymentDetails schema from Adyen API
layout: schema
name: PaymentDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The payment method type.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-details-schema.json
slug: checkout-payment-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-details-schema.json\",\n  \"title\": \"PaymentDetails\",\n  \"description\": \"PaymentDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The payment method type.\",\n      \"enum\": [\n        \"alipay\",\n        \"multibanco\",\n        \"bankTransfer_IBAN\",\n        \"paybright\",\n        \"paynow\",\n        \"affirm\",\n        \"affirm_pos\",\n        \"trustly\",\n        \"trustlyvector\",\n        \"oney\",\n        \"facilypay\",\n        \"facilypay_3x\",\n        \"facilypay_4x\",\n        \"facilypay_6x\",\n        \"facilypay_10x\",\n        \"facilypay_12x\"\
  ,\n        \"unionpay\",\n        \"kcp_banktransfer\",\n        \"kcp_payco\",\n        \"kcp_creditcard\",\n        \"wechatpaySDK\",\n        \"wechatpayQR\",\n        \"wechatpayWeb\",\n        \"molpay_boost\",\n        \"wallet_IN\",\n        \"payu_IN_cashcard\",\n        \"payu_IN_nb\",\n        \"upi_qr\",\n        \"paytm\",\n        \"molpay_ebanking_VN\",\n        \"paybybank\",\n        \"ebanking_FI\",\n        \"molpay_ebanking_MY\",\n        \"molpay_ebanking_direct_MY\",\n        \"swish\",\n        \"pix\",\n        \"walley\",\n        \"walley_b2b\",\n        \"alma\",\n        \"paypo\",\n        \"molpay_fpx\",\n        \"konbini\",\n        \"directEbanking\",\n        \"boletobancario\",\n        \"neteller\",\n        \"paysafecard\",\n        \"cashticket\",\n        \"ikano\",\n        \"karenmillen\",\n        \"oasis\",\n        \"warehouse\",\n        \"primeiropay_boleto\",\n        \"mada\",\n        \"benefit\",\n        \"knet\",\n        \"omannet\",\n\
  \        \"gopay_wallet\",\n        \"kcp_naverpay\",\n        \"onlinebanking_IN\",\n        \"fawry\",\n        \"atome\",\n        \"moneybookers\",\n        \"naps\",\n        \"nordea\",\n        \"boletobancario_bradesco\",\n        \"boletobancario_itau\",\n        \"boletobancario_santander\",\n        \"boletobancario_bancodobrasil\",\n        \"boletobancario_hsbc\",\n        \"molpay_maybank2u\",\n        \"molpay_cimb\",\n        \"molpay_rhb\",\n        \"molpay_amb\",\n        \"molpay_hlb\",\n        \"molpay_affin_epg\",\n        \"molpay_bankislam\",\n        \"molpay_publicbank\",\n        \"fpx_agrobank\",\n        \"touchngo\",\n        \"maybank2u_mae\",\n        \"duitnow\",\n        \"promptpay\",\n        \"twint_pos\",\n        \"alipay_hk\",\n        \"alipay_hk_web\",\n        \"alipay_hk_wap\",\n        \"alipay_wap\",\n        \"balanceplatform\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentDetails
---
