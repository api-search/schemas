---
description: This object is used when creating or updating content.
layout: schema
name: ContentBodyCreate
properties_list:
- description: The body of the content in the relevant format.
  name: value
  type: string
- description: The content format type. Set the value of this property to the name of the format being used, e.g. 'storage'.
  name: representation
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-body-create-schema.json
slug: atlassian-confluence-content-content-body-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentBodyCreate\",\n  \"type\": \"object\",\n  \"description\": \"This object is used when creating or updating content.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The body of the content in the relevant format.\"\n    },\n    \"representation\": {\n      \"type\": \"string\",\n      \"description\": \"The content format type. Set the value of this property to\\nthe name of the format being used, e.g. 'storage'.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-body-create-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentBodyCreate
---
