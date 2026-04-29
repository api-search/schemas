---
description: An audience export is a list of users in an audience at the time of the list's creation. One audience may have multiple audience exports created for different days.
layout: schema
name: AudienceExport
properties_list:
- description: 'Required. The audience resource name. This resource name identifies the audience being listed and is shared between the Analytics Data & Admin APIs. Format: `properties/{property}/audiences/{audience}'
  name: audience
  type: string
- description: Output only. The descriptive display name for this audience. For example, "Purchasers".
  name: audienceDisplayName
  type: string
- description: Output only. The time when CreateAudienceExport was called and the AudienceExport began the `CREATING` state.
  name: beginCreatingTime
  type: string
- description: Output only. The total quota tokens charged during creation of the AudienceExport. Because this token count is based on activity from the `CREATING` state, this tokens charged will be fixed once an Au
  name: creationQuotaTokensCharged
  type: integer
- description: Required. The dimensions requested and displayed in the query response.
  name: dimensions
  type: array
- description: Output only. Error message is populated when an audience export fails during creation. A common reason for such a failure is quota exhaustion.
  name: errorMessage
  type: string
- description: 'Output only. Identifier. The audience export resource name assigned during creation. This resource name identifies this `AudienceExport`. Format: `properties/{property}/audienceExports/{audience_expor'
  name: name
  type: string
- description: Output only. The percentage completed for this audience export ranging between 0 to 100.
  name: percentageCompleted
  type: number
- description: Output only. The total number of rows in the AudienceExport result.
  name: rowCount
  type: integer
- description: Output only. The current state for this AudienceExport.
  name: state
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-audience-export-schema.json
slug: data-api-audience-export
source_filename: data-api-audience-export-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-audience-export-schema.json\",\n  \"title\": \"AudienceExport\",\n  \"description\": \"An audience export is a list of users in an audience at the time of the list's creation. One audience may have multiple audience exports created for different days.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"audience\": {\n      \"description\": \"Required. The audience resource name. This resource name identifies the audience being listed and is shared between the Analytics Data & Admin APIs. Format: `properties/{property}/audiences/{audience}`\",\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"audienceDisplayName\": {\n      \"description\": \"Output only. The descriptive display name for this audience. For example, \\\"Purchasers\\\".\",\n      \"readOnly\"\
  : true,\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"beginCreatingTime\": {\n      \"description\": \"Output only. The time when CreateAudienceExport was called and the AudienceExport began the `CREATING` state.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"creationQuotaTokensCharged\": {\n      \"description\": \"Output only. The total quota tokens charged during creation of the AudienceExport. Because this token count is based on activity from the `CREATING` state, this tokens charged will be fixed once an AudienceExport enters the `ACTIVE` or `FAILED` states.\",\n      \"format\": \"int32\",\n      \"readOnly\": true,\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"dimensions\": {\n      \"description\": \"Required. The dimensions requested and displayed in the query response.\",\n      \"items\": {\n        \"description\"\
  : \"An audience dimension is a user attribute. Specific user attributed are requested and then later returned in the `QueryAudienceExportResponse`.\",\n        \"properties\": {\n          \"dimensionName\": {\n            \"description\": \"Optional. The API name of the dimension. See the [API Dimensions](https://developers.google.com/analytics/devguides/reporting/data/v1/audience-list-api-schema#dimensions) for the list of dimension names.\",\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"errorMessage\": {\n      \"description\": \"Output only. Error message is populated when an audience export fails during creation. A common reason for such a failure is quota exhaustion.\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Identifier. The audience export resource name assigned during\
  \ creation. This resource name identifies this `AudienceExport`. Format: `properties/{property}/audienceExports/{audience_export}`\",\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"percentageCompleted\": {\n      \"description\": \"Output only. The percentage completed for this audience export ranging between 0 to 100.\",\n      \"format\": \"double\",\n      \"readOnly\": true,\n      \"type\": \"number\",\n      \"example\": 75.5\n    },\n    \"rowCount\": {\n      \"description\": \"Output only. The total number of rows in the AudienceExport result.\",\n      \"format\": \"int32\",\n      \"readOnly\": true,\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"state\": {\n      \"description\": \"Output only. The current state for this AudienceExport.\",\n      \"enum\": [\n        \"STATE_UNSPECIFIED\",\n        \"CREATING\",\n        \"ACTIVE\",\n        \"FAILED\"\n      ],\n      \"readOnly\": true,\n  \
  \    \"type\": \"string\",\n      \"example\": \"STATE_UNSPECIFIED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-audience-export-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: AudienceExport
---
