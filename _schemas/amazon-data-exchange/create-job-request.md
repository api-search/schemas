---
description: Request body for creating a new job.
layout: schema
name: Create Job Request
properties_list:
- description: ''
  name: Type
  type: string
- description: ''
  name: Details
  type: object
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/create-job-request-schema.json
slug: create-job-request
source_filename: create-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/create-job-request-schema.json\",\n  \"title\": \"Create Job Request\",\n  \"description\": \"Request body for creating a new job.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Type\",\n    \"Details\"\n  ],\n  \"properties\": {\n    \"Type\": {\n      \"type\": \"string\"\n    },\n    \"Details\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/create-job-request-schema.json
tags:
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Create Job Request
---
