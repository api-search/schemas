---
description: A physical DeepRacer vehicle registered to an AWS account.
layout: schema
name: Car
properties_list:
- description: The ARN uniquely identifying the DeepRacer vehicle.
  name: vehicleArn
  type: string
- description: The display name of the vehicle.
  name: vehicleName
  type: string
- description: The ARN of the fleet this vehicle belongs to.
  name: fleetArn
  type: string
- description: Timestamp when the vehicle was registered.
  name: createdAt
  type: string
- description: Timestamp when the vehicle was last updated.
  name: lastModifiedTime
  type: string
- description: Tags associated with the vehicle.
  name: tagsList
  type: array
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/car-schema.json
slug: car
source_filename: car-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/car-schema.json\",\n  \"title\": \"Car\",\n  \"description\": \"A physical DeepRacer vehicle registered to an AWS account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN uniquely identifying the DeepRacer vehicle.\"\n    },\n    \"vehicleName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the vehicle.\"\n    },\n    \"fleetArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the fleet this vehicle belongs to.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the vehicle was registered.\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the vehicle was last updated.\"\n    },\n    \"tagsList\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the vehicle.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/car-schema.json
tags:
- Autonomous Vehicles
- Machine Learning
- Reinforcement Learning
- Robotics
title: Car
---
