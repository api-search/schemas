---
description: A Campaign Manager 360 ad. Ads define the creative content, delivery schedules, targeting rules, and placement assignments that control how advertising is served.
layout: schema
name: Ad
properties_list:
- description: Ad ID. Read-only, auto-generated field.
  name: id
  type: string
- description: Account ID of this ad.
  name: accountId
  type: string
- description: Subaccount ID of this ad.
  name: subaccountId
  type: string
- description: Campaign ID of this ad. Required on insert.
  name: campaignId
  type: string
- description: Advertiser ID of this ad. Required on insert.
  name: advertiserId
  type: string
- description: Name of this ad. Must be fewer than 256 characters.
  name: name
  type: string
- description: Whether this ad is active. Cannot be true when archived is true.
  name: active
  type: boolean
- description: Whether this ad is archived. Cannot be true when active is true.
  name: archived
  type: boolean
- description: Comments for this ad.
  name: comments
  type: string
- description: Date and time that this ad should start serving. Must be in the future for new ads.
  name: startTime
  type: string
- description: Date and time that this ad should stop serving. Must be after startTime.
  name: endTime
  type: string
- description: Type of ad. Required on insert.
  name: type
  type: string
- description: Whether this ad is a dynamic click tracker. Read-only after insert.
  name: dynamicClickTracker
  type: boolean
- description: Placement assignments for this ad.
  name: placementAssignments
  type: array
- description: Event tag overrides for this ad.
  name: eventTagOverrides
  type: array
- description: Identifies what kind of resource this is. Value is always dfareporting#ad.
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-ad-schema.json
slug: google-campaign-manager-ad
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ad\",\n  \"type\": \"object\",\n  \"description\": \"A Campaign Manager 360 ad. Ads define the creative content, delivery schedules, targeting rules, and placement assignments that control how advertising is served.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Ad ID. Read-only, auto-generated field.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID of this ad.\"\n    },\n    \"subaccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Subaccount ID of this ad.\"\n    },\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign ID of this ad. Required on insert.\"\n    },\n    \"advertiserId\": {\n      \"type\": \"string\",\n      \"description\": \"Advertiser ID of this ad. Required on insert.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Name of this ad. Must be fewer than 256 characters.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this ad is active. Cannot be true when archived is true.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this ad is archived. Cannot be true when active is true.\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Comments for this ad.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time that this ad should start serving. Must be in the future for new ads.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time that this ad should stop serving. Must be after startTime.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of ad. Required on insert.\"\n    },\n    \"dynamicClickTracker\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether this ad is a dynamic click tracker. Read-only after insert.\"\n    },\n    \"placementAssignments\": {\n      \"type\": \"array\",\n      \"description\": \"Placement assignments for this ad.\"\n    },\n    \"eventTagOverrides\": {\n      \"type\": \"array\",\n      \"description\": \"Event tag overrides for this ad.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies what kind of resource this is. Value is always dfareporting#ad.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-ad-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: Ad
---
