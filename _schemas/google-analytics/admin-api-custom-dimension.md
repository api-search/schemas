---
description: A definition for a CustomDimension.
layout: schema
name: CustomDimension
properties_list:
- description: Optional. Description for this custom dimension. Max length of 150 characters.
  name: description
  type: string
- description: Optional. If set to true, sets this dimension as NPA and excludes it from ads personalization. This is currently only supported by user-scoped custom dimensions.
  name: disallowAdsPersonalization
  type: boolean
- description: Required. Display name for this custom dimension as shown in the Analytics UI. Max length of 82 characters, alphanumeric plus space and underscore starting with a letter. Legacy system-generated displ
  name: displayName
  type: string
- description: 'Output only. Resource name for this CustomDimension resource. Format: properties/{property}/customDimensions/{customDimension}'
  name: name
  type: string
- description: Required. Immutable. Tagging parameter name for this custom dimension. If this is a user-scoped dimension, then this is the user property name. If this is an event-scoped dimension, then this is the e
  name: parameterName
  type: string
- description: Required. Immutable. The scope of this dimension.
  name: scope
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-custom-dimension-schema.json
slug: admin-api-custom-dimension
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-custom-dimension-schema.json\",\n  \"title\": \"CustomDimension\",\n  \"description\": \"A definition for a CustomDimension.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Optional. Description for this custom dimension. Max length of 150 characters.\",\n      \"type\": \"string\"\n    },\n    \"disallowAdsPersonalization\": {\n      \"description\": \"Optional. If set to true, sets this dimension as NPA and excludes it from ads personalization. This is currently only supported by user-scoped custom dimensions.\",\n      \"type\": \"boolean\"\n    },\n    \"displayName\": {\n      \"description\": \"Required. Display name for this custom dimension as shown in the Analytics UI. Max length of 82 characters, alphanumeric plus space and underscore\
  \ starting with a letter. Legacy system-generated display names may contain square brackets, but updates to this field will never permit square brackets.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Resource name for this CustomDimension resource. Format: properties/{property}/customDimensions/{customDimension}\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"parameterName\": {\n      \"description\": \"Required. Immutable. Tagging parameter name for this custom dimension. If this is a user-scoped dimension, then this is the user property name. If this is an event-scoped dimension, then this is the event parameter name. If this is an item-scoped dimension, then this is the parameter name found in the eCommerce items array. May only contain alphanumeric and underscore characters, starting with a letter. Max length of 24 characters for user-scoped dimensions, 40 characters for event-scoped dimensions.\",\n      \"\
  type\": \"string\"\n    },\n    \"scope\": {\n      \"description\": \"Required. Immutable. The scope of this dimension.\",\n      \"enum\": [\n        \"DIMENSION_SCOPE_UNSPECIFIED\",\n        \"EVENT\",\n        \"USER\",\n        \"ITEM\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-custom-dimension-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: CustomDimension
---
