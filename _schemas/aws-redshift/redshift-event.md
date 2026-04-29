---
description: Describes an event.
layout: schema
name: Event
properties_list:
- description: ''
  name: SourceIdentifier
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: EventCategories
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: Date
  type: object
- description: ''
  name: EventId
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-event-schema.json
slug: redshift-event
source_filename: redshift-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceIdentifier\": {},\n    \"SourceType\": {},\n    \"Message\": {},\n    \"EventCategories\": {},\n    \"Severity\": {},\n    \"Date\": {},\n    \"EventId\": {}\n  },\n  \"description\": \"Describes an event.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-event-schema.json\",\n  \"title\": \"Event\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-event-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: Event
---
