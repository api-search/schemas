---
description: A set of elements to filter the returned scheduled actions.
layout: schema
name: ScheduledActionFilter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Values
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-scheduled-action-filter-schema.json
slug: redshift-scheduled-action-filter
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {},\n    \"Values\": {}\n  },\n  \"required\": [\n    \"Name\",\n    \"Values\"\n  ],\n  \"description\": \"A set of elements to filter the returned scheduled actions. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-scheduled-action-filter-schema.json\",\n  \"title\": \"ScheduledActionFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-scheduled-action-filter-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ScheduledActionFilter
---
