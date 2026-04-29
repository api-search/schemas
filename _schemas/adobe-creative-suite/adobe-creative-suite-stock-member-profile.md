---
description: Adobe Stock member profile and account details
layout: schema
name: MemberProfile
properties_list:
- description: Core user account information
  name: stock_user
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-member-profile-schema.json
slug: adobe-creative-suite-stock-member-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-member-profile-schema.json\",\n  \"title\": \"MemberProfile\",\n  \"description\": \"Adobe Stock member profile and account details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stock_user\": {\n      \"type\": \"object\",\n      \"description\": \"Core user account information\",\n      \"properties\": {\n        \"nb_downloads\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of downloads by this member\"\n        },\n        \"nb_standard_downloads\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of standard license downloads\"\n        },\n        \"nb_standard_downloads_remaining\": {\n          \"type\": \"integer\",\n          \"description\": \"Remaining standard download quota\"\n        },\n \
  \       \"nb_standard_downloads_limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Total standard download limit for the current period\"\n        },\n        \"purchase_options\": {\n          \"type\": \"object\",\n          \"description\": \"Available purchase and licensing options for the member\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-member-profile-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: MemberProfile
---
