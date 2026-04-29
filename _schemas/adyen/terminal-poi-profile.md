---
description: POIProfile schema from Adyen API
layout: schema
name: POIProfile
properties_list:
- description: ''
  name: GenericProfile
  type: object
- description: ''
  name: ServiceProfiles
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-poi-profile-schema.json
slug: terminal-poi-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-profile-schema.json\",\n  \"title\": \"POIProfile\",\n  \"description\": \"POIProfile schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GenericProfile\": {\n      \"$ref\": \"#/components/schemas/GenericProfile\"\n    },\n    \"ServiceProfiles\": {\n      \"$ref\": \"#/components/schemas/ServiceProfiles\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-profile-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: POIProfile
---
