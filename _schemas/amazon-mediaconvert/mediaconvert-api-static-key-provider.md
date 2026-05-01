---
description: Use these settings to set up encryption with a static key provider.
layout: schema
name: StaticKeyProvider
properties_list:
- description: ''
  name: KeyFormat
  type: object
- description: ''
  name: KeyFormatVersions
  type: object
- description: ''
  name: StaticKeyValue
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-static-key-provider-schema.json
slug: mediaconvert-api-static-key-provider
source_filename: mediaconvert-api-static-key-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-static-key-provider-schema.json\",\n  \"title\": \"StaticKeyProvider\",\n  \"description\": \"Use these settings to set up encryption with a static key provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternIdentityAZaZ26AZaZ09163\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyFormat\"\n          },\n          \"description\": \"Relates to DRM implementation. Sets the value of the KEYFORMAT attribute. Must be 'identity' or a reverse DNS string. May be omitted to indicate an implicit value of 'identity'.\"\n        }\n      ]\n    },\n    \"KeyFormatVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternDD\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"keyFormatVersions\"\n          },\n          \"description\": \"Relates to DRM implementation. Either a single positive integer version value or a slash delimited list of version values (1/2/3).\"\n        }\n      ]\n    },\n    \"StaticKeyValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternAZaZ0932\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"staticKeyValue\"\n          },\n          \"description\": \"Relates to DRM implementation. Use a 32-character hexidecimal string to specify Key Value (StaticKeyValue).\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"Relates to DRM implementation. The location of the license server used for protecting\
  \ content.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-static-key-provider-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: StaticKeyProvider
---
