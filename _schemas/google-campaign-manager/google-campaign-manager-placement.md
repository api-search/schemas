---
description: A Campaign Manager 360 placement. Placements represent ad inventory on publisher sites and define the size, format, pricing, and location where ads can be served.
layout: schema
name: Placement
properties_list:
- description: Placement ID. Read-only, auto-generated field.
  name: id
  type: string
- description: Account ID of this placement.
  name: accountId
  type: string
- description: Subaccount ID of this placement.
  name: subaccountId
  type: string
- description: Advertiser ID of this placement.
  name: advertiserId
  type: string
- description: Campaign ID of this placement. Required on insert.
  name: campaignId
  type: string
- description: Name of this placement. Must be fewer than 512 characters.
  name: name
  type: string
- description: Site ID associated with this placement. Required on insert, read-only after.
  name: siteId
  type: string
- description: Directory site ID of this placement. Required on insert, read-only after.
  name: directorySiteId
  type: string
- description: External ID for this placement.
  name: externalId
  type: string
- description: Key name of this placement, auto-generated from the name.
  name: keyName
  type: string
- description: ID of the placement group this placement belongs to.
  name: placementGroupId
  type: string
- description: Placement compatibility. Required on insert.
  name: compatibility
  type: string
- description: Additional sizes associated with this placement.
  name: additionalSizes
  type: array
- description: Tag formats to generate for this placement.
  name: tagFormats
  type: array
- description: Payment source for this placement. Read-only after insert.
  name: paymentSource
  type: string
- description: Whether payment was approved for this placement. Read-only for non-publisher-paid placements.
  name: paymentApproved
  type: boolean
- description: Third-party placement status.
  name: status
  type: string
- description: Whether this placement is active, inactive, archived, or permanently archived.
  name: activeStatus
  type: string
- description: ID of the content category assigned to this placement.
  name: contentCategoryId
  type: string
- description: ID of the placement strategy assigned to this placement.
  name: placementStrategyId
  type: string
- description: Comments for this placement.
  name: comment
  type: string
- description: Whether this placement is the primary placement in a roadblock.
  name: primary
  type: boolean
- description: Whether creatives assigned to this placement must be SSL-compliant.
  name: sslRequired
  type: boolean
- description: Whether this placement opts out of ad blocking.
  name: adBlockingOptOut
  type: boolean
- description: Whether this placement opts out of tag wrapping.
  name: wrappingOptOut
  type: boolean
- description: Whether Verification and ActiveView for in-stream video creatives are disabled for this placement.
  name: videoActiveViewOptOut
  type: boolean
- description: VPAID adapter setting for this placement.
  name: vpaidAdapterChoice
  type: string
- description: Identifies what kind of resource this is. Value is always dfareporting#placement.
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-placement-schema.json
slug: google-campaign-manager-placement
source_filename: google-campaign-manager-placement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Placement\",\n  \"type\": \"object\",\n  \"description\": \"A Campaign Manager 360 placement. Placements represent ad inventory on publisher sites and define the size, format, pricing, and location where ads can be served.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Placement ID. Read-only, auto-generated field.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID of this placement.\"\n    },\n    \"subaccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Subaccount ID of this placement.\"\n    },\n    \"advertiserId\": {\n      \"type\": \"string\",\n      \"description\": \"Advertiser ID of this placement.\"\n    },\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign ID of this placement. Required on insert.\"\n    },\n    \"name\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Name of this placement. Must be fewer than 512 characters.\"\n    },\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"Site ID associated with this placement. Required on insert, read-only after.\"\n    },\n    \"directorySiteId\": {\n      \"type\": \"string\",\n      \"description\": \"Directory site ID of this placement. Required on insert, read-only after.\"\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External ID for this placement.\"\n    },\n    \"keyName\": {\n      \"type\": \"string\",\n      \"description\": \"Key name of this placement, auto-generated from the name.\"\n    },\n    \"placementGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the placement group this placement belongs to.\"\n    },\n    \"compatibility\": {\n      \"type\": \"string\",\n      \"description\": \"Placement compatibility. Required on insert.\"\n    },\n    \"additionalSizes\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Additional sizes associated with this placement.\"\n    },\n    \"tagFormats\": {\n      \"type\": \"array\",\n      \"description\": \"Tag formats to generate for this placement.\"\n    },\n    \"paymentSource\": {\n      \"type\": \"string\",\n      \"description\": \"Payment source for this placement. Read-only after insert.\"\n    },\n    \"paymentApproved\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether payment was approved for this placement. Read-only for non-publisher-paid placements.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Third-party placement status.\"\n    },\n    \"activeStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this placement is active, inactive, archived, or permanently archived.\"\n    },\n    \"contentCategoryId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the content category assigned to this placement.\"\
  \n    },\n    \"placementStrategyId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the placement strategy assigned to this placement.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comments for this placement.\"\n    },\n    \"primary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this placement is the primary placement in a roadblock.\"\n    },\n    \"sslRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether creatives assigned to this placement must be SSL-compliant.\"\n    },\n    \"adBlockingOptOut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this placement opts out of ad blocking.\"\n    },\n    \"wrappingOptOut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this placement opts out of tag wrapping.\"\n    },\n    \"videoActiveViewOptOut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Verification and ActiveView for\
  \ in-stream video creatives are disabled for this placement.\"\n    },\n    \"vpaidAdapterChoice\": {\n      \"type\": \"string\",\n      \"description\": \"VPAID adapter setting for this placement.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies what kind of resource this is. Value is always dfareporting#placement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-placement-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: Placement
---
