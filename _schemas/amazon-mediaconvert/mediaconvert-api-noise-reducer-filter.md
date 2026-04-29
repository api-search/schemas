---
description: Use Noise reducer filter (NoiseReducerFilter) to select one of the following spatial image filtering functions. To use this setting, you must also enable Noise reducer (NoiseReducer). * Bilateral preserves edges while reducing noise. * Mean (softest), Gaussian, Lanczos, and Sharpen (sharpest) do convolution filtering. * Conserve does min/max noise reduction. * Spatial does frequency-domain filtering based on JND principles. * Temporal optimizes video quality for complex motion.
layout: schema
name: NoiseReducerFilter
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-noise-reducer-filter-schema.json
slug: mediaconvert-api-noise-reducer-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-filter-schema.json\",\n  \"title\": \"NoiseReducerFilter\",\n  \"description\": \"Use Noise reducer filter (NoiseReducerFilter) to select one of the following spatial image filtering functions. To use this setting, you must also enable Noise reducer (NoiseReducer). * Bilateral preserves edges while reducing noise. * Mean (softest), Gaussian, Lanczos, and Sharpen (sharpest) do convolution filtering. * Conserve does min/max noise reduction. * Spatial does frequency-domain filtering based on JND principles. * Temporal optimizes video quality for complex motion.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"BILATERAL\",\n    \"MEAN\",\n    \"GAUSSIAN\",\n    \"LANCZOS\",\n    \"SHARPEN\",\n    \"CONSERVE\",\n    \"SPATIAL\",\n    \"TEMPORAL\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-noise-reducer-filter-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NoiseReducerFilter
---
