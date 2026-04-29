---
description: A key-value element that will be displayed along with the report.
layout: schema
name: report_data
properties_list:
- description: The type of data contained in the value field. If not provided, then the value will be detected as a boolean, number or string.
  name: type
  type: string
- description: A string describing what this data field represents.
  name: title
  type: string
- description: The value of the data element.
  name: value
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-report_data-schema.json
slug: atlassian-bitbucket-repositories-report_data
source_filename: atlassian-bitbucket-repositories-report_data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"report_data\",\n  \"type\": \"object\",\n  \"description\": \"A key-value element that will be displayed along with the report.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data contained in the value field. If not provided, then the value will be detected as a boolean, number or string.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A string describing what this data field represents.\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"The value of the data element.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-report_data-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: report_data
---
