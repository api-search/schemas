---
description: ''
layout: schema
name: AppAttributes
properties_list:
- description: The name of the app
  name: name
  type: string
- description: The bundle ID of the app
  name: bundleId
  type: string
- description: The SKU of the app
  name: sku
  type: string
- description: The primary locale for the app (e.g., en-US)
  name: primaryLocale
  type: string
- description: Whether the app is or was made for kids
  name: isOrEverWasMadeForKids
  type: boolean
- description: Declaration of whether the app uses third-party content
  name: contentRightsDeclaration
  type: string
- description: Whether streamlined purchasing is enabled
  name: streamlinedPurchasingEnabled
  type: boolean
- description: URL for subscription status notifications
  name: subscriptionStatusUrl
  type: '[''string'', ''null'']'
- description: URL for sandbox subscription status notifications
  name: subscriptionStatusUrlForSandbox
  type: '[''string'', ''null'']'
- description: Version of the subscription status URL
  name: subscriptionStatusUrlVersion
  type: '[''string'', ''null'']'
- description: Version of the sandbox subscription status URL
  name: subscriptionStatusUrlVersionForSandbox
  type: '[''string'', ''null'']'
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-app-attributes-schema.json
slug: app-store-connect-app-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the app\"\n    },\n    \"bundleId\": {\n      \"type\": \"string\",\n      \"description\": \"The bundle ID of the app\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"The SKU of the app\"\n    },\n    \"primaryLocale\": {\n      \"type\": \"string\",\n      \"description\": \"The primary locale for the app (e.g., en-US)\"\n    },\n    \"isOrEverWasMadeForKids\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the app is or was made for kids\"\n    },\n    \"contentRightsDeclaration\": {\n      \"type\": \"string\",\n      \"description\": \"Declaration of whether the app uses third-party content\"\n    },\n    \"streamlinedPurchasingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether streamlined purchasing is enabled\"\n    },\n    \"subscriptionStatusUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"URL for subscription status notifications\"\n    },\n    \"subscriptionStatusUrlForSandbox\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"URL for sandbox subscription status notifications\"\n    },\n    \"subscriptionStatusUrlVersion\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Version of the subscription status URL\"\n    },\n    \"subscriptionStatusUrlVersionForSandbox\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Version of the sandbox subscription status URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-app-attributes-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: AppAttributes
---
