---
description: Specify the strength of the Bandwidth reduction filter. For most workflows, we recommend that you choose Auto to reduce the bandwidth of your output with little to no perceptual decrease in video quality. For high quality and high bitrate outputs, choose Low. For the most bandwidth reduction, choose High. We recommend that you choose High for low bitrate outputs. Note that High may incur a slight increase in the softness of your output.
layout: schema
name: BandwidthReductionFilterStrength
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-bandwidth-reduction-filter-strength-schema.json
slug: mediaconvert-api-bandwidth-reduction-filter-strength
source_filename: mediaconvert-api-bandwidth-reduction-filter-strength-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-bandwidth-reduction-filter-strength-schema.json\",\n  \"title\": \"BandwidthReductionFilterStrength\",\n  \"description\": \"Specify the strength of the Bandwidth reduction filter. For most workflows, we recommend that you choose Auto to reduce the bandwidth of your output with little to no perceptual decrease in video quality. For high quality and high bitrate outputs, choose Low. For the most bandwidth reduction, choose High. We recommend that you choose High for low bitrate outputs. Note that High may incur a slight increase in the softness of your output.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"LOW\",\n    \"MEDIUM\",\n    \"HIGH\",\n    \"AUTO\",\n    false\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-bandwidth-reduction-filter-strength-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BandwidthReductionFilterStrength
---
