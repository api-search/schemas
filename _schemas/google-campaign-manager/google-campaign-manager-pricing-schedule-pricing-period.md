---
description: A pricing period within a pricing schedule.
layout: schema
name: PricingSchedulePricingPeriod
properties_list:
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: Units of this pricing period.
  name: units
  type: string
- description: Rate or cost of this pricing period in nanos.
  name: rateOrCostNanos
  type: string
- description: Comments for this pricing period.
  name: pricingComment
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-pricing-schedule-pricing-period-schema.json
slug: google-campaign-manager-pricing-schedule-pricing-period
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PricingSchedulePricingPeriod\",\n  \"type\": \"object\",\n  \"description\": \"A pricing period within a pricing schedule.\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"units\": {\n      \"type\": \"string\",\n      \"description\": \"Units of this pricing period.\"\n    },\n    \"rateOrCostNanos\": {\n      \"type\": \"string\",\n      \"description\": \"Rate or cost of this pricing period in nanos.\"\n    },\n    \"pricingComment\": {\n      \"type\": \"string\",\n      \"description\": \"Comments for this pricing period.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-pricing-schedule-pricing-period-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: PricingSchedulePricingPeriod
---
