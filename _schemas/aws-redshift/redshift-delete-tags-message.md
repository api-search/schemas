---
description: Contains the output from the <code>DeleteTags</code> action.
layout: schema
name: DeleteTagsMessage
properties_list:
- description: ''
  name: ResourceName
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-delete-tags-message-schema.json
slug: redshift-delete-tags-message
source_filename: redshift-delete-tags-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceName\": {},\n    \"TagKeys\": {}\n  },\n  \"required\": [\n    \"ResourceName\",\n    \"TagKeys\"\n  ],\n  \"description\": \"Contains the output from the <code>DeleteTags</code> action. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-delete-tags-message-schema.json\",\n  \"title\": \"DeleteTagsMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-delete-tags-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DeleteTagsMessage
---
