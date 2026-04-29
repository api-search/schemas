---
description: Response containing a list of DeepRacer vehicles.
layout: schema
name: ListCarsResponse
properties_list:
- description: List of DeepRacer vehicles.
  name: cars
  type: array
- description: Token for retrieving the next page of results.
  name: nextToken
  type: string
provider_name: Amazon DeepRacer
provider_slug: amazon-deepracer
schema_file: json-schema/list-cars-response-schema.json
slug: list-cars-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deepracer/json-schema/list-cars-response-schema.json\",\n  \"title\": \"ListCarsResponse\",\n  \"description\": \"Response containing a list of DeepRacer vehicles.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cars\": {\n      \"type\": \"array\",\n      \"description\": \"List of DeepRacer vehicles.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for retrieving the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deepracer/refs/heads/main/json-schema/list-cars-response-schema.json
tags:
- Autonomous Vehicles
- AWS
- Machine Learning
- Reinforcement Learning
- Robotics
title: ListCarsResponse
---
