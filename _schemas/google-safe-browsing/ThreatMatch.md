---
description: A threat match returned by the Google Safe Browsing API.
layout: schema
name: Google Safe Browsing Threat Match
properties_list:
- description: The type of threat.
  name: threatType
  type: string
- description: The platform type.
  name: platformType
  type: string
- description: The type of threat entry.
  name: threatEntryType
  type: string
- description: The threat entry.
  name: threat
  type: object
- description: Metadata associated with the threat entry.
  name: threatEntryMetadata
  type: object
- description: The cache duration for the returned match.
  name: cacheDuration
  type: string
provider_name: Google Safe Browsing
provider_slug: google-safe-browsing
schema_file: json-schema/ThreatMatch.json
slug: ThreatMatch
source_filename: ThreatMatch.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"ThreatMatch.json\",\n  \"title\": \"Google Safe Browsing Threat Match\",\n  \"description\": \"A threat match returned by the Google Safe Browsing API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threatType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of threat.\",\n      \"enum\": [\n        \"MALWARE\",\n        \"SOCIAL_ENGINEERING\",\n        \"UNWANTED_SOFTWARE\",\n        \"POTENTIALLY_HARMFUL_APPLICATION\",\n        \"THREAT_TYPE_UNSPECIFIED\"\n      ]\n    },\n    \"platformType\": {\n      \"type\": \"string\",\n      \"description\": \"The platform type.\",\n      \"enum\": [\n        \"WINDOWS\",\n        \"LINUX\",\n        \"ANDROID\",\n        \"OSX\",\n        \"IOS\",\n        \"ANY_PLATFORM\",\n        \"ALL_PLATFORMS\",\n        \"CHROME\",\n        \"PLATFORM_TYPE_UNSPECIFIED\"\n      ]\n    },\n    \"threatEntryType\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"The type of threat entry.\",\n      \"enum\": [\n        \"URL\",\n        \"EXECUTABLE\",\n        \"THREAT_ENTRY_TYPE_UNSPECIFIED\"\n      ]\n    },\n    \"threat\": {\n      \"type\": \"object\",\n      \"description\": \"The threat entry.\",\n      \"properties\": {\n        \"hash\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        },\n        \"digest\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"threatEntryMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata associated with the threat entry.\"\n    },\n    \"cacheDuration\": {\n      \"type\": \"string\",\n      \"description\": \"The cache duration for the returned match.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-safe-browsing/refs/heads/main/json-schema/ThreatMatch.json
tags:
- Google
- Malware
- Safe Browsing
- Security
- Threats
- URLs
title: Google Safe Browsing Threat Match
---
