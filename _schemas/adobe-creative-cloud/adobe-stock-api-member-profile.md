---
description: MemberProfile from Adobe API
layout: schema
name: MemberProfile
properties_list:
- description: ''
  name: available_entitlement
  type: object
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-stock-api-member-profile-schema.json
slug: adobe-stock-api-member-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-member-profile-schema.json\",\n  \"title\": \"MemberProfile\",\n  \"description\": \"MemberProfile from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"available_entitlement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"quota\": {\n          \"type\": \"integer\",\n          \"description\": \"Remaining download quota.\"\n        },\n        \"license_type_id\": {\n          \"type\": \"integer\"\n        },\n        \"has_credit_model\": {\n          \"type\": \"boolean\"\n        },\n        \"has_agency_model\": {\n          \"type\": \"boolean\"\n        },\n        \"is_cce\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the member has a Creative Cloud Enterprise plan.\"\n        },\n        \"full_entitlement_quota\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"standard_credits_quota\": {\n              \"type\": \"integer\"\n            },\n            \"premium_credits_quota\": {\n              \"type\": \"integer\"\n            },\n            \"universal_credits_quota\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-member-profile-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: MemberProfile
---
