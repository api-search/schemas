---
description: ConfigurationTag schema from Amazon Application Discovery Service API
layout: schema
name: ConfigurationTag
properties_list:
- description: A type of IT asset to tag.
  name: configurationType
  type: string
- description: The configuration ID for the item to tag.
  name: configurationId
  type: string
- description: A type of tag on which to filter.
  name: key
  type: string
- description: A value on which to filter.
  name: value
  type: string
- description: The time the configuration tag was created in Coordinated Universal Time (UTC).
  name: timeOfCreation
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-configuration-tag-schema.json
slug: application-discovery-service-configuration-tag
source_filename: application-discovery-service-configuration-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-configuration-tag-schema.json\",\n  \"title\": \"ConfigurationTag\",\n  \"description\": \"ConfigurationTag schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVER\",\n        \"PROCESS\",\n        \"CONNECTION\",\n        \"APPLICATION\"\n      ],\n      \"example\": \"SERVER\",\n      \"description\": \"A type of IT asset to tag.\"\n    },\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"example\": \"d-SERVER-500456\",\n      \"description\": \"The configuration ID for the item to tag.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"environment\",\n      \"description\"\
  : \"A type of tag on which to filter.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"production\",\n      \"description\": \"A value on which to filter.\"\n    },\n    \"timeOfCreation\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:00:00Z\",\n      \"description\": \"The time the configuration tag was created in Coordinated Universal Time (UTC).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-configuration-tag-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: ConfigurationTag
---
