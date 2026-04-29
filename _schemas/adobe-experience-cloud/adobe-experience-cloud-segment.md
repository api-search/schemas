---
description: An audience segment definition used across Adobe Experience Cloud products to target groups of profiles based on shared attributes, behaviors, or engagement patterns.
layout: schema
name: Adobe Experience Cloud Segment
properties_list:
- description: The unique identifier for the segment.
  name: segmentId
  type: string
- description: The human-readable name of the segment.
  name: name
  type: string
- description: A detailed description of what the segment represents.
  name: description
  type: string
- description: The segment definition expression.
  name: expression
  type: object
- description: How the segment is evaluated against profiles.
  name: evaluationType
  type: string
- description: The merge policy used when evaluating this segment.
  name: mergePolicyId
  type: string
- description: The XDM schema this segment is based on.
  name: schema
  type: object
- description: The current status of the segment.
  name: status
  type: string
- description: The estimated number of profiles in this segment.
  name: profileCount
  type: integer
- description: The user who created the segment.
  name: owner
  type: object
- description: Tags for organizing and categorizing segments.
  name: tags
  type: array
- description: When the segment was created.
  name: created
  type: string
- description: When the segment was last modified.
  name: lastModified
  type: string
- description: When the segment was last evaluated.
  name: lastEvaluated
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/adobe-experience-cloud-segment.json
slug: adobe-experience-cloud-segment
source_filename: adobe-experience-cloud-segment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"adobe-experience-cloud-segment.json\",\n  \"title\": \"Adobe Experience Cloud Segment\",\n  \"description\": \"An audience segment definition used across Adobe Experience Cloud products to target groups of profiles based on shared attributes, behaviors, or engagement patterns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"segmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the segment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the segment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of what the segment represents.\"\n    },\n    \"expression\": {\n      \"type\": \"object\",\n      \"description\": \"The segment definition expression.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"PQL\"],\n          \"description\": \"The expression language type.\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\"pql/text\", \"pql/json\"],\n          \"description\": \"The format of the expression value.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The PQL expression defining the segment criteria.\"\n        }\n      },\n      \"required\": [\"type\", \"value\"]\n    },\n    \"evaluationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"batch\", \"streaming\", \"edge\"],\n      \"description\": \"How the segment is evaluated against profiles.\"\n    },\n    \"mergePolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"The merge policy used when evaluating this segment.\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"The XDM schema this segment is based on.\",\n      \"properties\": {\n        \"name\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"realized\", \"failed\"],\n      \"description\": \"The current status of the segment.\"\n    },\n    \"profileCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The estimated number of profiles in this segment.\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"The user who created the segment.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags for organizing and categorizing segments.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the segment was created.\"\n    },\n  \
  \  \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the segment was last modified.\"\n    },\n    \"lastEvaluated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the segment was last evaluated.\"\n    }\n  },\n  \"required\": [\"segmentId\", \"name\", \"expression\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/adobe-experience-cloud-segment.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Adobe Experience Cloud Segment
---
