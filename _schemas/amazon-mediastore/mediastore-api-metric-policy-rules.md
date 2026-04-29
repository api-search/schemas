---
description: MetricPolicyRules schema from Amazon MediaStore API
layout: schema
name: MetricPolicyRules
properties_list: []
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-metric-policy-rules-schema.json
slug: mediastore-api-metric-policy-rules
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-metric-policy-rules-schema.json\",\n  \"title\": \"MetricPolicyRules\",\n  \"description\": \"MetricPolicyRules schema from Amazon MediaStore API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/MetricPolicyRule\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 300\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-metric-policy-rules-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MetricPolicyRules
---
