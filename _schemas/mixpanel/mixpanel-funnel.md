---
description: Represents a conversion funnel in Mixpanel, defining a sequence of events that users are expected to complete and measuring drop-off at each step.
layout: schema
name: Mixpanel Funnel
properties_list:
- description: Unique identifier for the funnel
  name: funnel_id
  type: integer
- description: Display name of the funnel
  name: name
  type: string
- description: Ordered sequence of funnel steps
  name: steps
  type: array
- description: Time window for funnel completion
  name: conversionWindow
  type: object
provider_name: Mixpanel
provider_slug: mixpanel
schema_file: json-schema/mixpanel-funnel-schema.json
slug: mixpanel-funnel
source_filename: mixpanel-funnel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.mixpanel.com/schemas/mixpanel/funnel.json\",\n  \"title\": \"Mixpanel Funnel\",\n  \"description\": \"Represents a conversion funnel in Mixpanel, defining a sequence of events that users are expected to complete and measuring drop-off at each step.\",\n  \"type\": \"object\",\n  \"required\": [\"funnel_id\", \"name\"],\n  \"properties\": {\n    \"funnel_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the funnel\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the funnel\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered sequence of funnel steps\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FunnelStep\"\n      },\n      \"minItems\": 2\n    },\n    \"conversionWindow\": {\n      \"type\": \"object\",\n      \"description\": \"Time window for funnel\
  \ completion\",\n      \"properties\": {\n        \"length\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Number of time units\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\"minute\", \"hour\", \"day\"],\n          \"description\": \"Time unit for the conversion window\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"FunnelStep\": {\n      \"type\": \"object\",\n      \"description\": \"A single step in a conversion funnel\",\n      \"properties\": {\n        \"event\": {\n          \"type\": \"string\",\n          \"description\": \"Event name for this step\"\n        },\n        \"count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of users who completed this step\"\n        },\n        \"avgTime\": {\n          \"type\": \"number\",\n          \"description\": \"Average time in seconds to reach this step from the previous step\"\
  \n        },\n        \"overallConversionRatio\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Conversion rate from step 1 to this step\"\n        },\n        \"stepConversionRatio\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Conversion rate from the previous step to this step\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/json-schema/mixpanel-funnel-schema.json
tags:
- Analytics
- Data Analysis
- Event Tracking
- Product Analytics
- User Behavior
title: Mixpanel Funnel
---
