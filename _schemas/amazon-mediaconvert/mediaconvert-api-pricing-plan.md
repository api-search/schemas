---
description: Specifies whether the pricing plan for the queue is on-demand or reserved. For on-demand, you pay per minute, billed in increments of .01 minute. For reserved, you pay for the transcoding capacity of the entire queue, regardless of how much or how little you use it. Reserved pricing requires a 12-month commitment.
layout: schema
name: PricingPlan
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-pricing-plan-schema.json
slug: mediaconvert-api-pricing-plan
source_filename: mediaconvert-api-pricing-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-pricing-plan-schema.json\",\n  \"title\": \"PricingPlan\",\n  \"description\": \"Specifies whether the pricing plan for the queue is on-demand or reserved. For on-demand, you pay per minute, billed in increments of .01 minute. For reserved, you pay for the transcoding capacity of the entire queue, regardless of how much or how little you use it. Reserved pricing requires a 12-month commitment.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ON_DEMAND\",\n    \"RESERVED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-pricing-plan-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PricingPlan
---
