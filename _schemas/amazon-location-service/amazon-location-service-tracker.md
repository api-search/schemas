---
description: An Amazon Location Service tracker resource for tracking device positions.
layout: schema
name: Tracker
properties_list:
- description: The name of the tracker resource.
  name: TrackerName
  type: string
- description: The Amazon Resource Name (ARN) for the tracker.
  name: TrackerArn
  type: string
- description: The optional description for the tracker resource.
  name: Description
  type: string
- description: The position filtering method of the tracker resource.
  name: PositionFiltering
  type: string
- description: The timestamp for when the tracker resource was created.
  name: CreateTime
  type: string
provider_name: Amazon Location Service
provider_slug: amazon-location-service
schema_file: json-schema/amazon-location-service-tracker-schema.json
slug: amazon-location-service-tracker
source_filename: amazon-location-service-tracker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/json-schema/amazon-location-service-tracker-schema.json\",\n  \"title\": \"Tracker\",\n  \"description\": \"An Amazon Location Service tracker resource for tracking device positions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TrackerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tracker resource.\",\n      \"example\": \"fleet-tracker\"\n    },\n    \"TrackerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the tracker.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The optional description for the tracker resource.\"\n    },\n    \"PositionFiltering\": {\n      \"type\": \"string\",\n      \"description\": \"The position filtering method of the tracker resource.\",\n  \
  \    \"example\": \"TimeBased\",\n      \"enum\": [\n        \"TimeBased\",\n        \"DistanceBased\",\n        \"AccuracyBased\"\n      ]\n    },\n    \"CreateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp for when the tracker resource was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-location-service/refs/heads/main/json-schema/amazon-location-service-tracker-schema.json
tags:
- Geocoding
- Geofencing
- Location
- Maps
- Routing
title: Tracker
---
