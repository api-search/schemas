---
description: A non-blocking warning or issue encountered during request processing.
layout: schema
name: Issue
properties_list:
- description: HTTP status code associated with the issue.
  name: status
  type: integer
- description: Application-specific error code.
  name: code
  type: integer
- description: Short description of the issue.
  name: title
  type: string
- description: Detailed explanation of the issue.
  name: detail
  type: string
- description: ''
  name: source
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-issue-schema.json
slug: airline-code-lookup-issue
source_filename: airline-code-lookup-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Issue\",\n  \"description\": \"A non-blocking warning or issue encountered during request processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code associated with the issue.\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Application-specific error code.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the issue.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed explanation of the issue.\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"pointer\": {\n          \"type\": \"string\",\n          \"description\": \"JSON pointer to the associated entity in the request.\"\n        },\n        \"parameter\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Name of the query parameter that caused the issue.\"\n        },\n        \"example\": {\n          \"type\": \"string\",\n          \"description\": \"Example of a valid value for the parameter.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-code-lookup-issue-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: Issue
---
