---
description: UpdatePaymentMethodInfo schema from Adyen API
layout: schema
name: UpdatePaymentMethodInfo
properties_list:
- description: Bancontact details.
  name: bcmc
  type: object
- description: Cartes Bancaires details.
  name: cartesBancaires
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
- description: Custom routing flags for acquirer routing.
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
- description: Indicates whether the payment method is enabled (**true**) or disabled (**false**).
  name: enabled
  type: boolean
- description: Girocard details.
  name: girocard
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
- description: Maestro details.
  name: maestro
  type: object
- description: MasterCard details.
  name: mc
  type: object
- description: The list of stores for this payment method
  name: storeIds
  type: array
- description: Visa details.
  name: visa
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-update-payment-method-info-schema.json
slug: management-update-payment-method-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-payment-method-info-schema.json\",\n  \"title\": \"UpdatePaymentMethodInfo\",\n  \"description\": \"UpdatePaymentMethodInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bcmc\": {\n      \"description\": \"Bancontact details.\",\n      \"$ref\": \"#/components/schemas/BcmcInfo\"\n    },\n    \"cartesBancaires\": {\n      \"description\": \"Cartes Bancaires details.\",\n      \"$ref\": \"#/components/schemas/CartesBancairesInfo\"\n    },\n    \"countries\": {\n      \"description\": \"The list of countries where a payment method is available. By default, all countries supported by the payment method.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"cup\": {\n      \"description\": \"China Union Pay details.\"\
  ,\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"currencies\": {\n      \"description\": \"The list of currencies that a payment method supports. By default, all currencies supported by the payment method.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"customRoutingFlags\": {\n      \"description\": \"Custom routing flags for acquirer routing.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"diners\": {\n      \"description\": \"Diners details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"discover\": {\n      \"description\": \"Discover details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"eftpos_australia\": {\n      \"description\": \"Eftpos Australia details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"enabled\": {\n      \"description\"\
  : \"Indicates whether the payment method is enabled (**true**) or disabled (**false**).\",\n      \"type\": \"boolean\"\n    },\n    \"girocard\": {\n      \"description\": \"Girocard details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"ideal\": {\n      \"description\": \"iDeal details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"interac_card\": {\n      \"description\": \"Interac Card details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"jcb\": {\n      \"description\": \"JCB details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"maestro\": {\n      \"description\": \"Maestro details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"mc\": {\n      \"description\": \"MasterCard details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    },\n    \"storeIds\": {\n      \"description\": \"The list\
  \ of stores for this payment method\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"visa\": {\n      \"description\": \"Visa details.\",\n      \"$ref\": \"#/components/schemas/GenericPmWithTdiInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-payment-method-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdatePaymentMethodInfo
---
