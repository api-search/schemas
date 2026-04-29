---
description: Contains the output from the <code>CreateTags</code> action.
layout: schema
name: CreateTagsMessage
properties_list:
- description: ''
  name: ResourceName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-tags-message-schema.json
slug: redshift-create-tags-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceName\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"ResourceName\",\n    \"Tags\"\n  ],\n  \"description\": \"Contains the output from the <code>CreateTags</code> action. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-tags-message-schema.json\",\n  \"title\": \"CreateTagsMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-tags-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateTagsMessage
---
