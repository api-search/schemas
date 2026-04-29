---
description: Request body for creating a new event action.
layout: schema
name: Create Event Action Request
properties_list:
- description: ''
  name: Event
  type: object
- description: ''
  name: Action
  type: object
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/create-event-action-request-schema.json
slug: create-event-action-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/create-event-action-request-schema.json\",\n  \"title\": \"Create Event Action Request\",\n  \"description\": \"Request body for creating a new event action.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Event\",\n    \"Action\"\n  ],\n  \"properties\": {\n    \"Event\": {\n      \"type\": \"object\"\n    },\n    \"Action\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/create-event-action-request-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Create Event Action Request
---
