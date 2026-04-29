---
description: A resource message representing a Google Analytics GA4 property.
layout: schema
name: Property
properties_list:
- description: 'Immutable. The resource name of the parent account Format: accounts/{account_id} Example: "accounts/123"'
  name: account
  type: string
- description: Output only. Time when the entity was originally created.
  name: createTime
  type: string
- description: 'The currency type used in reports involving monetary values. Format: https://en.wikipedia.org/wiki/ISO_4217 Examples: "USD", "EUR", "JPY"'
  name: currencyCode
  type: string
- description: Output only. If set, the time at which this property was trashed. If not set, then this property is not currently in the trash can.
  name: deleteTime
  type: string
- description: Required. Human-readable display name for this property. The max allowed display name length is 100 UTF-16 code units.
  name: displayName
  type: string
- description: Output only. If set, the time at which this trashed property will be permanently deleted. If not set, then this property is not currently in the trash can and is not slated to be deleted.
  name: expireTime
  type: string
- description: 'Industry associated with this property Example: AUTOMOTIVE, FOOD_AND_DRINK'
  name: industryCategory
  type: string
- description: 'Output only. Resource name of this property. Format: properties/{property_id} Example: "properties/1000"'
  name: name
  type: string
- description: 'Immutable. Resource name of this property''s logical parent. Note: The Property-Moving UI can be used to change the parent. Format: accounts/{account}, properties/{property} Example: "accounts/100", "p'
  name: parent
  type: string
- description: Immutable. The property type for this Property resource. When creating a property, if the type is "PROPERTY_TYPE_UNSPECIFIED", then "ORDINARY_PROPERTY" will be implied.
  name: propertyType
  type: string
- description: Output only. The Google Analytics service level that applies to this property.
  name: serviceLevel
  type: string
- description: 'Required. Reporting Time Zone, used as the day boundary for reports, regardless of where the data originates. If the time zone honors DST, Analytics will automatically adjust for the changes. NOTE: Ch'
  name: timeZone
  type: string
- description: Output only. Time when entity payload fields were last updated.
  name: updateTime
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-property-schema.json
slug: admin-api-property
source_filename: admin-api-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-property-schema.json\",\n  \"title\": \"Property\",\n  \"description\": \"A resource message representing a Google Analytics GA4 property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"description\": \"Immutable. The resource name of the parent account Format: accounts/{account_id} Example: \\\"accounts/123\\\"\",\n      \"type\": \"string\"\n    },\n    \"createTime\": {\n      \"description\": \"Output only. Time when the entity was originally created.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"description\": \"The currency type used in reports involving monetary values. Format: https://en.wikipedia.org/wiki/ISO_4217 Examples: \\\"USD\\\", \\\"EUR\\\", \\\"JPY\\\"\
  \",\n      \"type\": \"string\"\n    },\n    \"deleteTime\": {\n      \"description\": \"Output only. If set, the time at which this property was trashed. If not set, then this property is not currently in the trash can.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"Required. Human-readable display name for this property. The max allowed display name length is 100 UTF-16 code units.\",\n      \"type\": \"string\"\n    },\n    \"expireTime\": {\n      \"description\": \"Output only. If set, the time at which this trashed property will be permanently deleted. If not set, then this property is not currently in the trash can and is not slated to be deleted.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"industryCategory\": {\n      \"description\": \"Industry associated with this property Example: AUTOMOTIVE, FOOD_AND_DRINK\"\
  ,\n      \"enum\": [\n        \"INDUSTRY_CATEGORY_UNSPECIFIED\",\n        \"AUTOMOTIVE\",\n        \"BUSINESS_AND_INDUSTRIAL_MARKETS\",\n        \"FINANCE\",\n        \"HEALTHCARE\",\n        \"TECHNOLOGY\",\n        \"TRAVEL\",\n        \"OTHER\",\n        \"ARTS_AND_ENTERTAINMENT\",\n        \"BEAUTY_AND_FITNESS\",\n        \"BOOKS_AND_LITERATURE\",\n        \"FOOD_AND_DRINK\",\n        \"GAMES\",\n        \"HOBBIES_AND_LEISURE\",\n        \"HOME_AND_GARDEN\",\n        \"INTERNET_AND_TELECOM\",\n        \"LAW_AND_GOVERNMENT\",\n        \"NEWS\",\n        \"ONLINE_COMMUNITIES\",\n        \"PEOPLE_AND_SOCIETY\",\n        \"PETS_AND_ANIMALS\",\n        \"REAL_ESTATE\",\n        \"REFERENCE\",\n        \"SCIENCE\",\n        \"SPORTS\",\n        \"JOBS_AND_EDUCATION\",\n        \"SHOPPING\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Resource name of this property. Format: properties/{property_id} Example: \\\"properties/1000\\\"\"\
  ,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"parent\": {\n      \"description\": \"Immutable. Resource name of this property's logical parent. Note: The Property-Moving UI can be used to change the parent. Format: accounts/{account}, properties/{property} Example: \\\"accounts/100\\\", \\\"properties/101\\\"\",\n      \"type\": \"string\"\n    },\n    \"propertyType\": {\n      \"description\": \"Immutable. The property type for this Property resource. When creating a property, if the type is \\\"PROPERTY_TYPE_UNSPECIFIED\\\", then \\\"ORDINARY_PROPERTY\\\" will be implied.\",\n      \"enum\": [\n        \"PROPERTY_TYPE_UNSPECIFIED\",\n        \"PROPERTY_TYPE_ORDINARY\",\n        \"PROPERTY_TYPE_SUBPROPERTY\",\n        \"PROPERTY_TYPE_ROLLUP\"\n      ],\n      \"type\": \"string\"\n    },\n    \"serviceLevel\": {\n      \"description\": \"Output only. The Google Analytics service level that applies to this property.\",\n      \"enum\": [\n        \"SERVICE_LEVEL_UNSPECIFIED\"\
  ,\n        \"GOOGLE_ANALYTICS_STANDARD\",\n        \"GOOGLE_ANALYTICS_360\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"description\": \"Required. Reporting Time Zone, used as the day boundary for reports, regardless of where the data originates. If the time zone honors DST, Analytics will automatically adjust for the changes. NOTE: Changing the time zone only affects data going forward, and is not applied retroactively. Format: https://www.iana.org/time-zones Example: \\\"America/Los_Angeles\\\"\",\n      \"type\": \"string\"\n    },\n    \"updateTime\": {\n      \"description\": \"Output only. Time when entity payload fields were last updated.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-property-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Property
---
