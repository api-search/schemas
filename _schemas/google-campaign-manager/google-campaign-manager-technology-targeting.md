---
description: Technology targeting configuration.
layout: schema
name: TechnologyTargeting
properties_list:
- description: Browsers to target.
  name: browsers
  type: array
- description: Platforms to target.
  name: platforms
  type: array
- description: Operating systems to target.
  name: operatingSystems
  type: array
- description: Mobile carriers to target.
  name: mobileCarriers
  type: array
- description: Connection types to target.
  name: connectionTypes
  type: array
- description: Operating system versions to target.
  name: operatingSystemVersions
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-technology-targeting-schema.json
slug: google-campaign-manager-technology-targeting
source_filename: google-campaign-manager-technology-targeting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TechnologyTargeting\",\n  \"type\": \"object\",\n  \"description\": \"Technology targeting configuration.\",\n  \"properties\": {\n    \"browsers\": {\n      \"type\": \"array\",\n      \"description\": \"Browsers to target.\"\n    },\n    \"platforms\": {\n      \"type\": \"array\",\n      \"description\": \"Platforms to target.\"\n    },\n    \"operatingSystems\": {\n      \"type\": \"array\",\n      \"description\": \"Operating systems to target.\"\n    },\n    \"mobileCarriers\": {\n      \"type\": \"array\",\n      \"description\": \"Mobile carriers to target.\"\n    },\n    \"connectionTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Connection types to target.\"\n    },\n    \"operatingSystemVersions\": {\n      \"type\": \"array\",\n      \"description\": \"Operating system versions to target.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-technology-targeting-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: TechnologyTargeting
---
