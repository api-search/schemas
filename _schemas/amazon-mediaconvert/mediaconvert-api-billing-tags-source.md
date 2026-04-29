---
description: The tag type that AWS Billing and Cost Management will use to sort your AWS Elemental MediaConvert costs on any billing report that you set up.
layout: schema
name: BillingTagsSource
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-billing-tags-source-schema.json
slug: mediaconvert-api-billing-tags-source
source_filename: mediaconvert-api-billing-tags-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-billing-tags-source-schema.json\",\n  \"title\": \"BillingTagsSource\",\n  \"description\": \"The tag type that AWS Billing and Cost Management will use to sort your AWS Elemental MediaConvert costs on any billing report that you set up.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"QUEUE\",\n    \"PRESET\",\n    \"JOB_TEMPLATE\",\n    \"JOB\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-billing-tags-source-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BillingTagsSource
---
