---
description: The Bandwidth reduction filter increases the video quality of your output relative to its bitrate. Use to lower the bitrate of your constant quality QVBR output, with little or no perceptual decrease in quality. Or, use to increase the video quality of outputs with other rate control modes relative to the bitrate that you specify. Bandwidth reduction increases further when your input is low quality or noisy. Outputs that use this feature incur pro-tier pricing. When you include Bandwidth reduction filter, you cannot include the Noise reducer preprocessor.
layout: schema
name: BandwidthReductionFilter
properties_list:
- description: ''
  name: Sharpening
  type: object
- description: ''
  name: Strength
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-bandwidth-reduction-filter-schema.json
slug: mediaconvert-api-bandwidth-reduction-filter
source_filename: mediaconvert-api-bandwidth-reduction-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-bandwidth-reduction-filter-schema.json\",\n  \"title\": \"BandwidthReductionFilter\",\n  \"description\": \"The Bandwidth reduction filter increases the video quality of your output relative to its bitrate. Use to lower the bitrate of your constant quality QVBR output, with little or no perceptual decrease in quality. Or, use to increase the video quality of outputs with other rate control modes relative to the bitrate that you specify. Bandwidth reduction increases further when your input is low quality or noisy. Outputs that use this feature incur pro-tier pricing. When you include Bandwidth reduction filter, you cannot include the Noise reducer preprocessor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sharpening\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/BandwidthReductionFilterSharpening\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sharpening\"\n          },\n          \"description\": \"Optionally specify the level of sharpening to apply when you use the Bandwidth reduction filter.  Sharpening adds contrast to the edges of your video content and can reduce softness. Keep the default value Off to apply no sharpening. Set Sharpening strength to Low to apply a minimal amount of sharpening, or High to apply a maximum amount of sharpening.\"\n        }\n      ]\n    },\n    \"Strength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthReductionFilterStrength\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"strength\"\n          },\n          \"description\": \"Specify the strength of the Bandwidth reduction filter. For most workflows, we recommend that you choose Auto to reduce the bandwidth of your output with little to no perceptual\
  \ decrease in video quality. For high quality and high bitrate outputs, choose Low. For the most bandwidth reduction, choose High. We recommend that you choose High for low bitrate outputs. Note that High may incur a slight increase in the softness of your output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-bandwidth-reduction-filter-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BandwidthReductionFilter
---
