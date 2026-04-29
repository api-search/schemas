---
description: Specifies service specification with a stage file.
layout: schema
name: ServiceSpecStageFile
properties_list:
- description: Specifies the Snowflake internal stage where the specification file is stored; for example, @tutorial_stage.
  name: stage
  type: string
- description: Specifies the path to the service specification file on the stage; for example, 'some-dir/echo_spec.yaml'.
  name: spec_file
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-spec-stage-file-schema.json
slug: service-service-spec-stage-file
source_filename: service-service-spec-stage-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceSpecStageFile\",\n  \"type\": \"object\",\n  \"description\": \"Specifies service specification with a stage file.\",\n  \"properties\": {\n    \"stage\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the Snowflake internal stage where the specification file is stored; for example, @tutorial_stage.\"\n    },\n    \"spec_file\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the path to the service specification file on the stage; for example, 'some-dir/echo_spec.yaml'.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-spec-stage-file-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceSpecStageFile
---
