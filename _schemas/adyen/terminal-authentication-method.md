---
description: AuthenticationMethod schema from Adyen API
layout: schema
name: AuthenticationMethod
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-authentication-method-schema.json
slug: terminal-authentication-method
source_filename: terminal-authentication-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-authentication-method-schema.json\",\n  \"title\": \"AuthenticationMethod\",\n  \"description\": \"AuthenticationMethod schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"Bypass\",\n      \"ManualVerification\",\n      \"MerchantAuthentication\",\n      \"OfflinePIN\",\n      \"OnlinePIN\",\n      \"PaperSignature\",\n      \"SecureCertificate\",\n      \"SecureNoCertificate\",\n      \"SecuredChannel\",\n      \"SignatureCapture\",\n      \"UnknownMethod\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-authentication-method-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationMethod
---
