---
description: API_Entities_MetricImage model
layout: schema
name: API_Entities_MetricImage
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: filename
  type: string
- description: ''
  name: file_path
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: url_text
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-openapi-original-api_entities_metric-image-schema.json
slug: gitlab-openapi-original-api_entities_metric-image
source_filename: gitlab-openapi-original-api_entities_metric-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_metric-image-schema.json\",\n  \"title\": \"API_Entities_MetricImage\",\n  \"description\": \"API_Entities_MetricImage model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 23\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2020-11-13 00:06:18.084000+00:00\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"example\": \"file.png\"\n    },\n    \"file_path\": {\n      \"type\": \"string\",\n      \"example\": \"/uploads/-/system/alert_metric_image/file/23/file.png\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://example.com/metric\"\n    },\n    \"url_text\": {\n\
  \      \"type\": \"string\",\n      \"example\": \"An example metric\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_metric-image-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_MetricImage
---
