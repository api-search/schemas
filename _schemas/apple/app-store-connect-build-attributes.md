---
description: ''
layout: schema
name: BuildAttributes
properties_list:
- description: The build version string (CFBundleVersion)
  name: version
  type: string
- description: The date and time the build was uploaded
  name: uploadedDate
  type: string
- description: The date and time the build expires
  name: expirationDate
  type: string
- description: Whether the build has expired
  name: expired
  type: boolean
- description: The minimum OS version required
  name: minOsVersion
  type: string
- description: The minimum macOS system version
  name: lsMinimumSystemVersion
  type: string
- description: The computed minimum macOS version
  name: computedMinMacOsVersion
  type: string
- description: Token for the build's icon asset
  name: iconAssetToken
  type: object
- description: The processing state of the build
  name: processingState
  type: string
- description: The audience type for the build
  name: buildAudienceType
  type: string
- description: Whether the build uses non-exempt encryption
  name: usesNonExemptEncryption
  type: '[''boolean'', ''null'']'
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-build-attributes-schema.json
slug: app-store-connect-build-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The build version string (CFBundleVersion)\"\n    },\n    \"uploadedDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the build was uploaded\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the build expires\"\n    },\n    \"expired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the build has expired\"\n    },\n    \"minOsVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The minimum OS version required\"\n    },\n    \"lsMinimumSystemVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The minimum macOS system version\"\n    },\n    \"computedMinMacOsVersion\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The computed minimum macOS version\"\n    },\n    \"iconAssetToken\": {\n      \"type\": \"object\",\n      \"description\": \"Token for the build's icon asset\"\n    },\n    \"processingState\": {\n      \"type\": \"string\",\n      \"description\": \"The processing state of the build\"\n    },\n    \"buildAudienceType\": {\n      \"type\": \"string\",\n      \"description\": \"The audience type for the build\"\n    },\n    \"usesNonExemptEncryption\": {\n      \"type\": \"['boolean', 'null']\",\n      \"description\": \"Whether the build uses non-exempt encryption\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-build-attributes-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: BuildAttributes
---
