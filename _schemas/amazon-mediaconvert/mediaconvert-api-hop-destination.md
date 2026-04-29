---
description: Optional. Configuration for a destination queue to which the job can hop once a customer-defined minimum wait time has passed.
layout: schema
name: HopDestination
properties_list:
- description: ''
  name: Priority
  type: object
- description: ''
  name: Queue
  type: object
- description: ''
  name: WaitMinutes
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hop-destination-schema.json
slug: mediaconvert-api-hop-destination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hop-destination-schema.json\",\n  \"title\": \"HopDestination\",\n  \"description\": \"Optional. Configuration for a destination queue to which the job can hop once a customer-defined minimum wait time has passed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative50Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priority\"\n          },\n          \"description\": \"Optional. When you set up a job to use queue hopping, you can specify a different relative priority for the job in the destination queue. If you don't specify, the relative priority will remain the same as in the previous queue.\"\n        }\n      ]\n    },\n    \"Queue\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queue\"\n          },\n          \"description\": \"Optional unless the job is submitted on the default queue. When you set up a job to use queue hopping, you can specify a destination queue. This queue cannot be the original queue to which the job is submitted. If the original queue isn't the default queue and you don't specify the destination queue, the job will move to the default queue.\"\n        }\n      ]\n    },\n    \"WaitMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"waitMinutes\"\n          },\n          \"description\": \"Required for setting up a job to use queue hopping. Minimum wait time in minutes until the job can hop to the destination queue. Valid range is 1 to 4320 minutes, inclusive.\"\n   \
  \     }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hop-destination-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HopDestination
---
