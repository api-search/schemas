---
description: A customer journey definition in Adobe Journey Optimizer representing an orchestrated sequence of actions, conditions, and wait steps that guide individual profiles through personalized multi-channel experiences.
layout: schema
name: Adobe Experience Cloud Journey
properties_list:
- description: The unique identifier for the journey.
  name: journeyId
  type: string
- description: The human-readable name of the journey.
  name: name
  type: string
- description: A description of the journey purpose and flow.
  name: description
  type: string
- description: The current lifecycle status of the journey.
  name: status
  type: string
- description: The version identifier of the journey.
  name: version
  type: string
- description: The conditions under which profiles enter the journey.
  name: entryCondition
  type: object
- description: The ordered list of activities in the journey.
  name: activities
  type: array
- description: Execution metrics for the journey.
  name: metrics
  type: object
- description: When the journey was created.
  name: created
  type: string
- description: When the journey was last modified.
  name: lastModified
  type: string
- description: When the journey was last published.
  name: publishedAt
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/adobe-experience-cloud-journey.json
slug: adobe-experience-cloud-journey
source_filename: adobe-experience-cloud-journey.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"adobe-experience-cloud-journey.json\",\n  \"title\": \"Adobe Experience Cloud Journey\",\n  \"description\": \"A customer journey definition in Adobe Journey Optimizer representing an orchestrated sequence of actions, conditions, and wait steps that guide individual profiles through personalized multi-channel experiences.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"journeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the journey.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the journey.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the journey purpose and flow.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"live\", \"stopped\", \"closed\", \"finished\"],\n      \"description\"\
  : \"The current lifecycle status of the journey.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version identifier of the journey.\"\n    },\n    \"entryCondition\": {\n      \"type\": \"object\",\n      \"description\": \"The conditions under which profiles enter the journey.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"segment\", \"event\", \"audience\"],\n          \"description\": \"The type of entry trigger.\"\n        },\n        \"segmentId\": {\n          \"type\": \"string\",\n          \"description\": \"The segment ID for segment-based entry.\"\n        },\n        \"eventId\": {\n          \"type\": \"string\",\n          \"description\": \"The event ID for event-based entry.\"\n        },\n        \"schedule\": {\n          \"type\": \"object\",\n          \"description\": \"Scheduling configuration for recurring journeys.\",\n          \"properties\": {\n            \"frequency\"\
  : {\n              \"type\": \"string\",\n              \"enum\": [\"once\", \"daily\", \"weekly\", \"monthly\"]\n            },\n            \"startDate\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            },\n            \"endDate\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            }\n          }\n        }\n      }\n    },\n    \"activities\": {\n      \"type\": \"array\",\n      \"description\": \"The ordered list of activities in the journey.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"activityId\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for this activity step.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"action\", \"condition\", \"wait\", \"end\", \"email\", \"push\", \"sms\", \"customAction\"],\n            \"description\": \"The type of journey\
  \ activity.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"A label for this activity step.\"\n          },\n          \"configuration\": {\n            \"type\": \"object\",\n            \"description\": \"Type-specific configuration for the activity.\"\n          },\n          \"nextActivityId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the next activity in the flow.\"\n          }\n        },\n        \"required\": [\"activityId\", \"type\"]\n      }\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Execution metrics for the journey.\",\n      \"properties\": {\n        \"totalEntered\": {\n          \"type\": \"integer\",\n          \"description\": \"Total profiles that have entered the journey.\"\n        },\n        \"currentlyInJourney\": {\n          \"type\": \"integer\",\n          \"description\": \"Profiles currently progressing through the journey.\"\
  \n        },\n        \"totalExited\": {\n          \"type\": \"integer\",\n          \"description\": \"Profiles that have completed or exited the journey.\"\n        },\n        \"totalErrored\": {\n          \"type\": \"integer\",\n          \"description\": \"Profiles that encountered errors.\"\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the journey was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the journey was last modified.\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the journey was last published.\"\n    }\n  },\n  \"required\": [\"journeyId\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/adobe-experience-cloud-journey.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Adobe Experience Cloud Journey
---
