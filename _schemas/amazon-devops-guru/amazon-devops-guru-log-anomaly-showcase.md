---
description: A cluster of similar anomalous log events found within a log group.
layout: schema
name: LogAnomalyShowcase
properties_list:
- description: ''
  name: LogAnomalyClasses
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-log-anomaly-showcase-schema.json
slug: amazon-devops-guru-log-anomaly-showcase
source_filename: amazon-devops-guru-log-anomaly-showcase-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-log-anomaly-showcase-schema.json\",\n  \"title\": \"LogAnomalyShowcase\",\n  \"description\": \"A cluster of similar anomalous log events found within a log group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogAnomalyClasses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogAnomalyClasses\"\n        },\n        {\n          \"description\": \" A list of anomalous log events that may be related. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-log-anomaly-showcase-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: LogAnomalyShowcase
---
