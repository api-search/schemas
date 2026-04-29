---
description: A link between a GA4 property and a Google Ads account.
layout: schema
name: GoogleAdsLink
properties_list:
- description: Enable personalized advertising features with this integration. Automatically publish my Google Analytics audience lists and Google Analytics remarketing events/parameters to the linked Google Ads acc
  name: adsPersonalizationEnabled
  type: boolean
- description: Output only. If true, this link is for a Google Ads manager account.
  name: canManageClients
  type: boolean
- description: Output only. Time when this link was originally created.
  name: createTime
  type: string
- description: Output only. Email address of the user that created the link. An empty string will be returned if the email address can't be retrieved.
  name: creatorEmailAddress
  type: string
- description: Immutable. Google Ads customer ID.
  name: customerId
  type: string
- description: 'Output only. Format: properties/{propertyId}/googleAdsLinks/{googleAdsLinkId} Note: googleAdsLinkId is not the Google Ads customer ID.'
  name: name
  type: string
- description: Output only. Time when this link was last updated.
  name: updateTime
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-google-ads-link-schema.json
slug: admin-api-google-ads-link
source_filename: admin-api-google-ads-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-google-ads-link-schema.json\",\n  \"title\": \"GoogleAdsLink\",\n  \"description\": \"A link between a GA4 property and a Google Ads account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adsPersonalizationEnabled\": {\n      \"description\": \"Enable personalized advertising features with this integration. Automatically publish my Google Analytics audience lists and Google Analytics remarketing events/parameters to the linked Google Ads account. If this field is not set on create/update, it will be defaulted to true.\",\n      \"type\": \"boolean\"\n    },\n    \"canManageClients\": {\n      \"description\": \"Output only. If true, this link is for a Google Ads manager account.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"createTime\": {\n      \"description\"\
  : \"Output only. Time when this link was originally created.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"creatorEmailAddress\": {\n      \"description\": \"Output only. Email address of the user that created the link. An empty string will be returned if the email address can't be retrieved.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"customerId\": {\n      \"description\": \"Immutable. Google Ads customer ID.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Format: properties/{propertyId}/googleAdsLinks/{googleAdsLinkId} Note: googleAdsLinkId is not the Google Ads customer ID.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"updateTime\": {\n      \"description\": \"Output only. Time when this link was last updated.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-google-ads-link-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: GoogleAdsLink
---
