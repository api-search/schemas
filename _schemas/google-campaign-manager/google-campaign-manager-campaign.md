---
description: A Campaign Manager 360 campaign. Campaigns are the top-level organizational unit for advertising activities, grouping ads, placements, and creatives under a single advertiser with shared configuration, date ranges, and targeting.
layout: schema
name: Campaign
properties_list:
- description: Campaign ID. This is a read-only, auto-generated field.
  name: id
  type: string
- description: Account ID of this campaign.
  name: accountId
  type: string
- description: Subaccount ID of this campaign.
  name: subaccountId
  type: string
- description: Advertiser ID of this campaign. Required on insert.
  name: advertiserId
  type: string
- description: Advertiser group ID of the associated advertiser.
  name: advertiserGroupId
  type: string
- description: Name of this campaign. Must be fewer than 512 characters and unique among campaigns of the same advertiser.
  name: name
  type: string
- description: Whether this campaign has been archived.
  name: archived
  type: boolean
- description: Start date of this campaign. The date format is YYYY-MM-DD.
  name: startDate
  type: string
- description: End date of this campaign. Must be on or after the start date. The date format is YYYY-MM-DD.
  name: endDate
  type: string
- description: Arbitrary comments about this campaign. Must be fewer than 256 characters.
  name: comment
  type: string
- description: Billing invoice code included in the invoices.
  name: billingInvoiceCode
  type: string
- description: Default landing page ID for this campaign.
  name: defaultLandingPageId
  type: string
- description: External ID for this campaign.
  name: externalId
  type: string
- description: Audience segment groups assigned to this campaign. Maximum of 300 segment groups.
  name: audienceSegmentGroups
  type: array
- description: Event tag overrides for this campaign.
  name: eventTagOverrides
  type: array
- description: List of creative group IDs assigned to this campaign.
  name: creativeGroupIds
  type: array
- description: Additional creative optimization configurations.
  name: additionalCreativeOptimizationConfigurations
  type: array
- description: EU political advertising declaration for this campaign.
  name: euPoliticalAdsDeclaration
  type: string
- description: Identifies what kind of resource this is. Value is always dfareporting#campaign.
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-campaign-schema.json
slug: google-campaign-manager-campaign
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Campaign\",\n  \"type\": \"object\",\n  \"description\": \"A Campaign Manager 360 campaign. Campaigns are the top-level organizational unit for advertising activities, grouping ads, placements, and creatives under a single advertiser with shared configuration, date ranges, and targeting.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign ID. This is a read-only, auto-generated field.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID of this campaign.\"\n    },\n    \"subaccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Subaccount ID of this campaign.\"\n    },\n    \"advertiserId\": {\n      \"type\": \"string\",\n      \"description\": \"Advertiser ID of this campaign. Required on insert.\"\n    },\n    \"advertiserGroupId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Advertiser group ID of the associated advertiser.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of this campaign. Must be fewer than 512 characters and unique among campaigns of the same advertiser.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this campaign has been archived.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date of this campaign. The date format is YYYY-MM-DD.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"End date of this campaign. Must be on or after the start date. The date format is YYYY-MM-DD.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary comments about this campaign. Must be fewer than 256 characters.\"\n    },\n    \"billingInvoiceCode\": {\n      \"type\": \"string\",\n      \"description\": \"Billing invoice code included in the invoices.\"\
  \n    },\n    \"defaultLandingPageId\": {\n      \"type\": \"string\",\n      \"description\": \"Default landing page ID for this campaign.\"\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External ID for this campaign.\"\n    },\n    \"audienceSegmentGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Audience segment groups assigned to this campaign. Maximum of 300 segment groups.\"\n    },\n    \"eventTagOverrides\": {\n      \"type\": \"array\",\n      \"description\": \"Event tag overrides for this campaign.\"\n    },\n    \"creativeGroupIds\": {\n      \"type\": \"array\",\n      \"description\": \"List of creative group IDs assigned to this campaign.\"\n    },\n    \"additionalCreativeOptimizationConfigurations\": {\n      \"type\": \"array\",\n      \"description\": \"Additional creative optimization configurations.\"\n    },\n    \"euPoliticalAdsDeclaration\": {\n      \"type\": \"string\",\n      \"description\": \"EU political\
  \ advertising declaration for this campaign.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies what kind of resource this is. Value is always dfareporting#campaign.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-campaign-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: Campaign
---
