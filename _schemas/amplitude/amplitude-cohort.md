---
description: Schema for an Amplitude behavioral cohort representing a group of users defined by shared behavioral patterns or properties.
layout: schema
name: Amplitude Cohort
properties_list:
- description: The unique identifier for the cohort.
  name: id
  type: string
- description: The name of the cohort.
  name: name
  type: string
- description: A description of the cohort and the behavioral pattern it captures.
  name: description
  type: string
- description: The number of users currently in the cohort.
  name: size
  type: integer
- description: The date and time the cohort membership was last computed.
  name: lastComputed
  type: string
- description: Whether the cohort has been archived.
  name: archived
  type: boolean
- description: The email address of the cohort owner.
  name: owner
  type: string
- description: The Amplitude project ID the cohort belongs to.
  name: appId
  type: integer
- description: ''
  name: definition
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/amplitude-cohort-schema.json
slug: amplitude-cohort
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://amplitude.com/schemas/amplitude/cohort.json\",\n  \"title\": \"Amplitude Cohort\",\n  \"description\": \"Schema for an Amplitude behavioral cohort representing a group of users defined by shared behavioral patterns or properties.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the cohort.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cohort.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the cohort and the behavioral pattern it captures.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of users currently in the cohort.\",\n      \"minimum\": 0\n    },\n\
  \    \"lastComputed\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the cohort membership was last computed.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cohort has been archived.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the cohort owner.\"\n    },\n    \"appId\": {\n      \"type\": \"integer\",\n      \"description\": \"The Amplitude project ID the cohort belongs to.\"\n    },\n    \"definition\": {\n      \"$ref\": \"#/$defs/CohortDefinition\"\n    }\n  },\n  \"$defs\": {\n    \"CohortDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"The behavioral definition that determines cohort membership.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of cohort definition.\",\n          \"enum\"\
  : [\"behavioral\", \"property\", \"uploaded\"]\n        },\n        \"events\": {\n          \"type\": \"array\",\n          \"description\": \"Array of event conditions that define behavioral cohort membership.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/EventCondition\"\n          }\n        },\n        \"properties\": {\n          \"type\": \"array\",\n          \"description\": \"Array of user property conditions for property-based cohorts.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PropertyCondition\"\n          }\n        }\n      }\n    },\n    \"EventCondition\": {\n      \"type\": \"object\",\n      \"description\": \"A condition based on user event behavior.\",\n      \"properties\": {\n        \"event_type\": {\n          \"type\": \"string\",\n          \"description\": \"The event type the condition evaluates.\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator.\",\n\
  \          \"enum\": [\"is\", \"is_not\", \"contains\", \"does_not_contain\", \"greater_than\", \"less_than\"]\n        },\n        \"value\": {\n          \"description\": \"The value to compare against.\"\n        }\n      }\n    },\n    \"PropertyCondition\": {\n      \"type\": \"object\",\n      \"description\": \"A condition based on user properties.\",\n      \"properties\": {\n        \"property\": {\n          \"type\": \"string\",\n          \"description\": \"The user property name.\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator.\",\n          \"enum\": [\"is\", \"is_not\", \"contains\", \"does_not_contain\", \"set\", \"not_set\", \"greater_than\", \"less_than\"]\n        },\n        \"value\": {\n          \"description\": \"The value to compare against.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/amplitude-cohort-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Amplitude Cohort
---
