---
description: ''
layout: schema
name: UserProperty
properties_list:
- description: ''
  name: key
  type: string
- description: The value of the content property.
  name: value
  type: object
- description: a unique identifier for the user property
  name: id
  type: string
- description: datetime when the property was last modified such as `2022-02-01T12:00:00.111Z`
  name: lastModifiedDate
  type: string
- description: datetime when the property was created such as `2022-01-01T12:00:00.111Z`
  name: createdDate
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-user-user-property-schema.json
slug: atlassian-confluence-user-user-property
source_filename: atlassian-confluence-user-user-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserProperty\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"The value of the content property.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"a unique identifier for the user property\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"datetime when the property was last modified such as `2022-02-01T12:00:00.111Z`\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"datetime when the property was created such as `2022-01-01T12:00:00.111Z`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-user-user-property-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: UserProperty
---
