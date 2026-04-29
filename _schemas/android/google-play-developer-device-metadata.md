---
description: Metadata about the device used to write a review.
layout: schema
name: DeviceMetadata
properties_list:
- description: Device manufacturer (e.g., Samsung, Google).
  name: manufacturer
  type: string
- description: Device class (e.g., phone, tablet).
  name: deviceClass
  type: string
- description: Screen width in pixels.
  name: screenWidthPx
  type: integer
- description: Screen height in pixels.
  name: screenHeightPx
  type: integer
- description: Comma-separated list of native platforms (e.g., armeabi-v7a, arm64-v8a).
  name: nativePlatform
  type: string
- description: Device product name.
  name: productName
  type: string
- description: Screen density in DPI.
  name: screenDensityDpi
  type: integer
- description: OpenGL ES version.
  name: glEsVersion
  type: integer
- description: CPU model identifier.
  name: cpuModel
  type: string
- description: CPU manufacturer.
  name: cpuMake
  type: string
- description: Device RAM in megabytes.
  name: ramMb
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-device-metadata-schema.json
slug: google-play-developer-device-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceMetadata\",\n  \"type\": \"object\",\n  \"description\": \"Metadata about the device used to write a review.\",\n  \"properties\": {\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Device manufacturer (e.g., Samsung, Google).\"\n    },\n    \"deviceClass\": {\n      \"type\": \"string\",\n      \"description\": \"Device class (e.g., phone, tablet).\"\n    },\n    \"screenWidthPx\": {\n      \"type\": \"integer\",\n      \"description\": \"Screen width in pixels.\"\n    },\n    \"screenHeightPx\": {\n      \"type\": \"integer\",\n      \"description\": \"Screen height in pixels.\"\n    },\n    \"nativePlatform\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of native platforms (e.g., armeabi-v7a, arm64-v8a).\"\n    },\n    \"productName\": {\n      \"type\": \"string\",\n      \"description\": \"Device product name.\"\n  \
  \  },\n    \"screenDensityDpi\": {\n      \"type\": \"integer\",\n      \"description\": \"Screen density in DPI.\"\n    },\n    \"glEsVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"OpenGL ES version.\"\n    },\n    \"cpuModel\": {\n      \"type\": \"string\",\n      \"description\": \"CPU model identifier.\"\n    },\n    \"cpuMake\": {\n      \"type\": \"string\",\n      \"description\": \"CPU manufacturer.\"\n    },\n    \"ramMb\": {\n      \"type\": \"integer\",\n      \"description\": \"Device RAM in megabytes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-device-metadata-schema.json
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
title: DeviceMetadata
---
