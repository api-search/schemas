---
description: Delivery schedule configuration for an ad, controlling pacing and priority.
layout: schema
name: DeliverySchedule
properties_list:
- description: Impression ratio for this ad. Used to calculate the relative weight of this ad vs other ads with the same priority.
  name: impressionRatio
  type: string
- description: Serving priority of this delivery schedule.
  name: priority
  type: string
- description: Whether or not hard cutoff is enabled. If true, the ad will not serve after the end time.
  name: hardCutoff
  type: boolean
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-delivery-schedule-schema.json
slug: google-campaign-manager-delivery-schedule
source_filename: google-campaign-manager-delivery-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeliverySchedule\",\n  \"type\": \"object\",\n  \"description\": \"Delivery schedule configuration for an ad, controlling pacing and priority.\",\n  \"properties\": {\n    \"impressionRatio\": {\n      \"type\": \"string\",\n      \"description\": \"Impression ratio for this ad. Used to calculate the relative weight of this ad vs other ads with the same priority.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Serving priority of this delivery schedule.\"\n    },\n    \"hardCutoff\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not hard cutoff is enabled. If true, the ad will not serve after the end time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-delivery-schedule-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: DeliverySchedule
---
