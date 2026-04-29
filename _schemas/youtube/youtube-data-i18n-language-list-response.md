---
description: A list of i18n language resources supported by the YouTube website.
layout: schema
name: I18nLanguageListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#i18nLanguageListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: A list of supported i18n languages.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-i18n-language-list-response-schema.json
slug: youtube-data-i18n-language-list-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of i18n language resources supported by the YouTube website.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#i18nLanguageListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of supported i18n languages.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's type. Value is youtube#i18nLanguage.\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag\
  \ of this resource.\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID uniquely identifying the i18n language.\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"The snippet object contains basic details about the i18n language.\",\n            \"properties\": {\n              \"hl\": {\n                \"type\": \"string\",\n                \"description\": \"A BCP-47 code that uniquely identifies a language.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the language as it is written in the language itself.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"I18nLanguageListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-i18n-language-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: I18nLanguageListResponse
---
