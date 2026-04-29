---
description: Selects DeveloperMetadata that matches all of the specified fields.
layout: schema
name: DeveloperMetadataLookup
properties_list:
- description: Limits the selected developer metadata to that which has a matching location type.
  name: locationType
  type: string
- description: Determines how this lookup matches the location.
  name: locationMatchingStrategy
  type: string
- description: Limits the selected developer metadata to that which has a matching metadata ID.
  name: metadataId
  type: integer
- description: Limits the selected developer metadata to that which has a matching metadata key.
  name: metadataKey
  type: string
- description: Limits the selected developer metadata to that which has a matching metadata value.
  name: metadataValue
  type: string
- description: Limits the selected developer metadata to that which has a matching visibility.
  name: visibility
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-developer-metadata-lookup-schema.json
slug: google-sheets-developer-metadata-lookup
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeveloperMetadataLookup\",\n  \"type\": \"object\",\n  \"description\": \"Selects DeveloperMetadata that matches all of the specified fields.\",\n  \"properties\": {\n    \"locationType\": {\n      \"type\": \"string\",\n      \"description\": \"Limits the selected developer metadata to that which has a matching location type.\"\n    },\n    \"locationMatchingStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"Determines how this lookup matches the location.\"\n    },\n    \"metadataId\": {\n      \"type\": \"integer\",\n      \"description\": \"Limits the selected developer metadata to that which has a matching metadata ID.\"\n    },\n    \"metadataKey\": {\n      \"type\": \"string\",\n      \"description\": \"Limits the selected developer metadata to that which has a matching metadata key.\"\n    },\n    \"metadataValue\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Limits the selected developer metadata to that which has a matching metadata value.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Limits the selected developer metadata to that which has a matching visibility.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-developer-metadata-lookup-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DeveloperMetadataLookup
---
