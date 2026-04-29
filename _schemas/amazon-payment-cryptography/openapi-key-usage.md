---
description: KeyUsage schema from Amazon Payment Cryptography
layout: schema
name: KeyUsage
properties_list: []
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
schema_file: json-schema/openapi-key-usage-schema.json
slug: openapi-key-usage
source_filename: openapi-key-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-usage-schema.json\",\n  \"title\": \"KeyUsage\",\n  \"description\": \"KeyUsage schema from Amazon Payment Cryptography\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"TR31_B0_BASE_DERIVATION_KEY\",\n    \"TR31_C0_CARD_VERIFICATION_KEY\",\n    \"TR31_D0_SYMMETRIC_DATA_ENCRYPTION_KEY\",\n    \"TR31_D1_ASYMMETRIC_KEY_FOR_DATA_ENCRYPTION\",\n    \"TR31_E0_EMV_MKEY_APP_CRYPTOGRAMS\",\n    \"TR31_E1_EMV_MKEY_CONFIDENTIALITY\",\n    \"TR31_E2_EMV_MKEY_INTEGRITY\",\n    \"TR31_E4_EMV_MKEY_DYNAMIC_NUMBERS\",\n    \"TR31_E5_EMV_MKEY_CARD_PERSONALIZATION\",\n    \"TR31_E6_EMV_MKEY_OTHER\",\n    \"TR31_K0_KEY_ENCRYPTION_KEY\",\n    \"TR31_K1_KEY_BLOCK_PROTECTION_KEY\",\n    \"TR31_K3_ASYMMETRIC_KEY_FOR_KEY_AGREEMENT\",\n    \"TR31_M3_ISO_9797_3_MAC_KEY\",\n    \"TR31_M6_ISO_9797_5_CMAC_KEY\"\
  ,\n    \"TR31_M7_HMAC_KEY\",\n    \"TR31_P0_PIN_ENCRYPTION_KEY\",\n    \"TR31_P1_PIN_GENERATION_KEY\",\n    \"TR31_S0_ASYMMETRIC_KEY_FOR_DIGITAL_SIGNATURE\",\n    \"TR31_V1_IBM3624_PIN_VERIFICATION_KEY\",\n    \"TR31_V2_VISA_PIN_VERIFICATION_KEY\",\n    \"TR31_K2_TR34_ASYMMETRIC_KEY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/json-schema/openapi-key-usage-schema.json
tags:
- AWS
- Cryptography
- Financial Services
- Payment Processing
- PCI
title: KeyUsage
---
