---
description: A curated Advisor topic that groups related rules and recommendations.
layout: schema
name: Topic
properties_list:
- description: The name of the topic.
  name: name
  type: string
- description: The URL-friendly slug for the topic.
  name: slug
  type: string
- description: A description of the topic.
  name: description
  type: string
- description: The tag associated with the topic.
  name: tag
  type: string
- description: Whether the topic is featured.
  name: featured
  type: boolean
- description: The number of systems impacted by rules in this topic.
  name: impacted_systems_count
  type: integer
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-topic-schema.json
slug: red-hat-insights-topic
source_filename: red-hat-insights-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Topic\",\n  \"type\": \"object\",\n  \"description\": \"A curated Advisor topic that groups related rules and recommendations.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the topic.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug for the topic.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the topic.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"The tag associated with the topic.\"\n    },\n    \"featured\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the topic is featured.\"\n    },\n    \"impacted_systems_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of systems impacted by rules in this topic.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-topic-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Topic
---
