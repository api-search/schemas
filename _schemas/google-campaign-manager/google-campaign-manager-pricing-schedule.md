---
description: Pricing schedule for a placement.
layout: schema
name: PricingSchedule
properties_list:
- description: Placement start date.
  name: startDate
  type: string
- description: Placement end date.
  name: endDate
  type: string
- description: Placement pricing type.
  name: pricingType
  type: string
- description: Placement cap cost type.
  name: capCostType
  type: string
- description: Pricing periods for this placement.
  name: pricingPeriods
  type: array
- description: Testing start date of this placement.
  name: testingStartDate
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-pricing-schedule-schema.json
slug: google-campaign-manager-pricing-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PricingSchedule\",\n  \"type\": \"object\",\n  \"description\": \"Pricing schedule for a placement.\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Placement start date.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"Placement end date.\"\n    },\n    \"pricingType\": {\n      \"type\": \"string\",\n      \"description\": \"Placement pricing type.\"\n    },\n    \"capCostType\": {\n      \"type\": \"string\",\n      \"description\": \"Placement cap cost type.\"\n    },\n    \"pricingPeriods\": {\n      \"type\": \"array\",\n      \"description\": \"Pricing periods for this placement.\"\n    },\n    \"testingStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Testing start date of this placement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-pricing-schedule-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: PricingSchedule
---
