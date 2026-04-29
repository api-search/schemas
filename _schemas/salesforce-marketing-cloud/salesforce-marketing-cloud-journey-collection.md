---
description: Paginated collection of journeys
layout: schema
name: JourneyCollection
properties_list:
- description: Total number of journeys matching the query
  name: count
  type: integer
- description: Current page number
  name: page
  type: integer
- description: Number of items per page
  name: pageSize
  type: integer
- description: ''
  name: items
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-collection-schema.json
slug: salesforce-marketing-cloud-journey-collection
source_filename: salesforce-marketing-cloud-journey-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JourneyCollection\",\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of journeys\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of journeys matching the query\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items per page\"\n    },\n    \"items\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-collection-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: JourneyCollection
---
