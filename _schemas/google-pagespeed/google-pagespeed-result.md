---
description: Schema for the response from the PageSpeed Insights API, containing Lighthouse audit scores, Core Web Vitals metrics, and optimization recommendations.
layout: schema
name: PageSpeed Insights Result
properties_list:
- description: The URL that was analyzed
  name: id
  type: string
- description: ''
  name: loadingExperience
  type: object
- description: ''
  name: originLoadingExperience
  type: object
- description: ''
  name: lighthouseResult
  type: object
- description: UTC timestamp of when the analysis was run
  name: analysisUTCTimestamp
  type: string
provider_name: Google PageSpeed
provider_slug: google-pagespeed
schema_file: json-schema/google-pagespeed-result-schema.json
slug: google-pagespeed-result
source_filename: google-pagespeed-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://googleapis.com/schemas/pagespeed/result.json\",\n  \"title\": \"PageSpeed Insights Result\",\n  \"description\": \"Schema for the response from the PageSpeed Insights API, containing Lighthouse audit scores, Core Web Vitals metrics, and optimization recommendations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that was analyzed\"\n    },\n    \"loadingExperience\": {\n      \"$ref\": \"#/$defs/LoadingExperience\"\n    },\n    \"originLoadingExperience\": {\n      \"$ref\": \"#/$defs/LoadingExperience\"\n    },\n    \"lighthouseResult\": {\n      \"$ref\": \"#/$defs/LighthouseResult\"\n    },\n    \"analysisUTCTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp of when the analysis was run\"\n    }\n  },\n  \"$defs\"\
  : {\n    \"LoadingExperience\": {\n      \"type\": \"object\",\n      \"description\": \"Chrome User Experience Report field data for the page or origin\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"metrics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"LARGEST_CONTENTFUL_PAINT_MS\": {\n              \"$ref\": \"#/$defs/Metric\"\n            },\n            \"FIRST_INPUT_DELAY_MS\": {\n              \"$ref\": \"#/$defs/Metric\"\n            },\n            \"CUMULATIVE_LAYOUT_SHIFT_SCORE\": {\n              \"$ref\": \"#/$defs/Metric\"\n            },\n            \"INTERACTION_TO_NEXT_PAINT\": {\n              \"$ref\": \"#/$defs/Metric\"\n            },\n            \"FIRST_CONTENTFUL_PAINT_MS\": {\n              \"$ref\": \"#/$defs/Metric\"\n            }\n          }\n        },\n        \"overall_category\": {\n          \"type\": \"string\",\n          \"enum\": [\"FAST\", \"AVERAGE\", \"SLOW\"\
  , \"NONE\"]\n        }\n      }\n    },\n    \"Metric\": {\n      \"type\": \"object\",\n      \"description\": \"A Core Web Vitals metric with distribution data\",\n      \"properties\": {\n        \"percentile\": {\n          \"type\": \"integer\",\n          \"description\": \"The metric value at the 75th percentile\"\n        },\n        \"distributions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"min\": { \"type\": \"integer\" },\n              \"max\": { \"type\": \"integer\" },\n              \"proportion\": { \"type\": \"number\" }\n            }\n          }\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"enum\": [\"FAST\", \"AVERAGE\", \"SLOW\"]\n        }\n      }\n    },\n    \"LighthouseResult\": {\n      \"type\": \"object\",\n      \"description\": \"Lighthouse audit results\",\n      \"properties\": {\n        \"requestedUrl\": {\n      \
  \    \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"finalUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"lighthouseVersion\": {\n          \"type\": \"string\"\n        },\n        \"fetchTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"categories\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"performance\": { \"$ref\": \"#/$defs/Category\" },\n            \"accessibility\": { \"$ref\": \"#/$defs/Category\" },\n            \"best-practices\": { \"$ref\": \"#/$defs/Category\" },\n            \"seo\": { \"$ref\": \"#/$defs/Category\" }\n          }\n        },\n        \"audits\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/Audit\"\n          }\n        }\n      }\n    },\n    \"Category\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\":\
  \ { \"type\": \"string\" },\n        \"title\": { \"type\": \"string\" },\n        \"score\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Category score from 0 to 1\"\n        }\n      }\n    },\n    \"Audit\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"title\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"score\": { \"type\": \"number\" },\n        \"displayValue\": { \"type\": \"string\" },\n        \"numericValue\": { \"type\": \"number\" },\n        \"numericUnit\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/json-schema/google-pagespeed-result-schema.json
tags:
- Core Web Vitals
- Google
- Lighthouse
- Page Speed
- SEO
- Web Performance
title: PageSpeed Insights Result
---
