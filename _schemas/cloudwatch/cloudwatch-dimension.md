---
description: A dimension is a name/value pair that is part of the identity of a metric.
layout: schema
name: Dimension
properties_list:
- description: The name of the dimension. Dimension names must contain only ASCII characters, must include at least one non-whitespace character, and cannot start with a colon (:).
  name: Name
  type: string
- description: The value of the dimension. Dimension values must contain only ASCII characters and must include at least one non-whitespace character.
  name: Value
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-dimension-schema.json
slug: cloudwatch-dimension
source_filename: cloudwatch-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dimension\",\n  \"type\": \"object\",\n  \"description\": \"A dimension is a name/value pair that is part of the identity of a metric.\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dimension. Dimension names must contain only ASCII characters, must include at least one non-whitespace character, and cannot start with a colon (:).\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the dimension. Dimension values must contain only ASCII characters and must include at least one non-whitespace character.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-dimension-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: Dimension
---
