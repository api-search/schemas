---
description: Optional field, defaults to DEFAULT. Specify DEFAULT for this operation to return your endpoints if any exist, or to create an endpoint for you and return it if one doesn't already exist. Specify GET_ONLY to return your endpoints if any exist, or an empty list if none exist.
layout: schema
name: DescribeEndpointsMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-describe-endpoints-mode-schema.json
slug: mediaconvert-api-describe-endpoints-mode
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-describe-endpoints-mode-schema.json\",\n  \"title\": \"DescribeEndpointsMode\",\n  \"description\": \"Optional field, defaults to DEFAULT. Specify DEFAULT for this operation to return your endpoints if any exist, or to create an endpoint for you and return it if one doesn't already exist. Specify GET_ONLY to return your endpoints if any exist, or an empty list if none exist.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DEFAULT\",\n    \"GET_ONLY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-describe-endpoints-mode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeEndpointsMode
---
