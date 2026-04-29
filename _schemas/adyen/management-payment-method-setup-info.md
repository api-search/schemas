---
description: PaymentMethodSetupInfo schema from Adyen API
layout: schema
name: PaymentMethodSetupInfo
properties_list:
- description: Afterpay Touch details.
  name: afterpayTouch
  type: object
- description: Apple Pay details.
  name: applePay
  type: object
- description: Bancontact details.
  name: bcmc
  type: object
- description: The unique identifier of the business line. Required if you have a [platform setup](https://docs.adyen.com/marketplaces-and-platforms/platform-structure-resources/platform-setup/).
  name: businessLineId
  type: string
- description: Cartes Bancaires details.
  name: cartesBancaires
  type: object
- description: Clearpay details.
  name: clearpay
  type: object
- description: The list of countries where a payment method is available. By default, all countries supported by the payment method.
  name: countries
  type: array
- description: China Union Pay details.
  name: cup
  type: object
- description: The list of currencies that a payment method supports. By default, all currencies supported by the payment method.
  name: currencies
  type: array
- description: The list of custom routing flags to route payment to the intended acquirer.
  name: customRoutingFlags
  type: array
- description: Diners details.
  name: diners
  type: object
- description: Discover details.
  name: discover
  type: object
- description: Eftpos Australia details.
  name: eftpos_australia
  type: object
- description: giropay details.
  name: giroPay
  type: object
- description: Girocard details.
  name: girocard
  type: object
- description: Google Pay details.
  name: googlePay
  type: object
- description: iDeal details.
  name: ideal
  type: object
- description: Interac Card details.
  name: interac_card
  type: object
- description: JCB details.
  name: jcb
  type: object
- description: Klarna details.
  name: klarna
  type: object
- description: Maestro details.
  name: maestro
  type: object
- description: MasterCard details.
  name: mc
  type: object
- description: Meal Voucher FR details.
  name: mealVoucher_FR
  type: object
- description: PayPal details.
  name: paypal
  type: object
- description: Your reference for the payment method. Supported characters a-z, A-Z, 0-9.
  name: reference
  type: string
- description: 'The sales channel. Required if the merchant account does not have a sales channel. When you provide this field, it overrides the default sales channel set on the merchant account. Possible values: **e'
  name: shopperInteraction
  type: string
- description: Sofort details.
  name: sofort
  type: object
- description: The unique identifier of the store for which to configure the payment method, if any.
  name: storeIds
  type: array
- description: Swish details.
  name: swish
  type: object
- description: Twint details.
  name: twint
  type: object
- description: Payment method [variant](https://docs.adyen.com/development-resources/paymentmethodvariant#management-api).
  name: type
  type: string
- description: Vipps details.
  name: vipps
  type: object
- description: Visa details.
  name: visa
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-payment-method-setup-info-schema.json
slug: management-payment-method-setup-info
source_filename: management-payment-method-setup-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payment-method-setup-info-schema.json\",\n  \"title\": \"PaymentMethodSetupInfo\",\n  \"description\": \"PaymentMethodSetupInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"afterpayTouch\": {\n      \"description\": \"Afterpay Touch details.\",\n      \"$ref\": \"#/components/schemas/AfterpayTouchInfo\"\n    },\n    \"applePay\": {\n      \"description\": \"Apple Pay details.\",\n      \"$ref\": \"#/components/schemas/ApplePayInfo\"\n    },\n    \"bcmc\": {\n      \"description\": \"Bancontact details.\",\n      \"$ref\": \"#/components/schemas/BcmcInfo\"\n    },\n    \"businessLineId\": {\n      \"description\": \"The unique identifier of the business line. Required if you have a [platform setup](https://docs.adyen.com/marketplaces-and-platforms/platform-structure-resources/platform-setup/).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"cartesBancaires\": {\n      \"description\": \"Cartes Bancaires details.\",\n      \"$ref\": \"#/components/schemas/CartesBancairesInfo\"\n    },\n    \"clearpay\": {\n      \"description\": \"Clearpay details.\",\n      \"$ref\": \"#/components/schemas/ClearpayInfo\"\n    },\n    \"countries\": {\n      \"description\": \"The list of countries where a payment method is available. By default, all countries supported by the payment method.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"cup\": {\n      \"description\": \"China Union Pay details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"currencies\": {\n      \"description\": \"The list of currencies that a payment method supports. By default, all currencies supported by the payment method.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"customRoutingFlags\"\
  : {\n      \"description\": \"The list of custom routing flags to route payment to the intended acquirer.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"diners\": {\n      \"description\": \"Diners details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"discover\": {\n      \"description\": \"Discover details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"eftpos_australia\": {\n      \"description\": \"Eftpos Australia details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"giroPay\": {\n      \"description\": \"giropay details.\",\n      \"$ref\": \"#/components/schemas/GiroPayInfo\"\n    },\n    \"girocard\": {\n      \"description\": \"Girocard details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"googlePay\": {\n      \"description\": \"Google Pay details.\",\n      \"$ref\": \"#/components/schemas/GooglePayInfo\"\
  \n    },\n    \"ideal\": {\n      \"description\": \"iDeal details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"interac_card\": {\n      \"description\": \"Interac Card details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"jcb\": {\n      \"description\": \"JCB details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"klarna\": {\n      \"description\": \"Klarna details.\",\n      \"$ref\": \"#/components/schemas/KlarnaInfo\"\n    },\n    \"maestro\": {\n      \"description\": \"Maestro details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"mc\": {\n      \"description\": \"MasterCard details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"mealVoucher_FR\": {\n      \"description\": \"Meal Voucher FR details.\",\n      \"$ref\": \"#/components/schemas/MealVoucherFRInfo\"\n    },\n    \"paypal\": {\n      \"description\"\
  : \"PayPal details.\",\n      \"$ref\": \"#/components/schemas/PayPalInfo\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment method. Supported characters a-z, A-Z, 0-9.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"The sales channel. Required if the merchant account does not have a sales channel. When you provide this field, it overrides the default sales channel set on the merchant account.\\n\\nPossible values: **eCommerce**, **pos**, **contAuth**, and **moto**. \",\n      \"enum\": [\n        \"eCommerce\",\n        \"pos\",\n        \"moto\",\n        \"contAuth\"\n      ],\n      \"type\": \"string\"\n    },\n    \"sofort\": {\n      \"description\": \"Sofort details.\",\n      \"$ref\": \"#/components/schemas/SofortInfo\"\n    },\n    \"storeIds\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The unique identifier of the store for which to configure\
  \ the payment method, if any.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"swish\": {\n      \"description\": \"Swish details.\",\n      \"$ref\": \"#/components/schemas/SwishInfo\"\n    },\n    \"twint\": {\n      \"description\": \"Twint details.\",\n      \"$ref\": \"#/components/schemas/TwintInfo\"\n    },\n    \"type\": {\n      \"description\": \"Payment method [variant](https://docs.adyen.com/development-resources/paymentmethodvariant#management-api).\",\n      \"enum\": [\n        \"afterpaytouch\",\n        \"alipay\",\n        \"alipay_hk\",\n        \"amex\",\n        \"applepay\",\n        \"bcmc\",\n        \"blik\",\n        \"cartebancaire\",\n        \"clearpay\",\n        \"cup\",\n        \"diners\",\n        \"directdebit_GB\",\n        \"discover\",\n        \"ebanking_FI\",\n        \"eftpos_australia\",\n        \"elo\",\n        \"elocredit\",\n        \"elodebit\",\n        \"girocard\",\n        \"googlepay\"\
  ,\n        \"hiper\",\n        \"hipercard\",\n        \"ideal\",\n        \"interac_card\",\n        \"jcb\",\n        \"klarna\",\n        \"klarna_account\",\n        \"klarna_paynow\",\n        \"maestro\",\n        \"mbway\",\n        \"mc\",\n        \"mcdebit\",\n        \"mealVoucher_FR\",\n        \"mobilepay\",\n        \"multibanco\",\n        \"onlineBanking_PL\",\n        \"paybybank\",\n        \"paypal\",\n        \"payshop\",\n        \"swish\",\n        \"trustly\",\n        \"twint\",\n        \"twint_pos\",\n        \"vipps\",\n        \"visa\",\n        \"visadebit\",\n        \"vpay\",\n        \"wechatpay\",\n        \"wechatpay_pos\"\n      ],\n      \"type\": \"string\"\n    },\n    \"vipps\": {\n      \"description\": \"Vipps details.\",\n      \"$ref\": \"#/components/schemas/VippsInfo\"\n    },\n    \"visa\": {\n      \"description\": \"Visa details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    }\n  },\n  \"required\": [\n    \"type\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payment-method-setup-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentMethodSetupInfo
---
