---
description: MfaVerifyResponse schema from Bandwidth mfa API
layout: schema
name: MfaVerifyResponse
properties_list:
- description: Whether the MFA code is valid and has not expired
  name: valid
  type: boolean
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/mfa-mfa-verify-response-schema.json
slug: mfa-mfa-verify-response
source_filename: mfa-mfa-verify-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-verify-response-schema.json\",\n  \"title\": \"MfaVerifyResponse\",\n  \"description\": \"MfaVerifyResponse schema from Bandwidth mfa API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the MFA code is valid and has not expired\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/mfa-mfa-verify-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MfaVerifyResponse
---
