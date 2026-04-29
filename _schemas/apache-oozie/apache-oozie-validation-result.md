---
description: Result of XML definition validation.
layout: schema
name: ValidationResult
properties_list:
- description: Validation outcome.
  name: validate
  type: object
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-validation-result-schema.json
slug: apache-oozie-validation-result
source_filename: apache-oozie-validation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-validation-result-schema.json\",\n  \"title\": \"ValidationResult\",\n  \"description\": \"Result of XML definition validation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"validate\": {\n      \"type\": \"object\",\n      \"description\": \"Validation outcome.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Validation status.\",\n          \"example\": \"valid\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-validation-result-schema.json
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: ValidationResult
---
