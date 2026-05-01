---
description: Template version source data.
layout: schema
name: TemplateVersionSourceInput
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-template-version-source-input-schema.json
slug: amazon-proton-template-version-source-input
source_filename: amazon-proton-template-version-source-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-template-version-source-input-schema.json\",\n  \"title\": \"TemplateVersionSourceInput\",\n  \"description\": \"Template version source data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectSource\"\n        },\n        {\n          \"description\": \"An S3 source object that includes the template bundle S3 path and name for a template minor version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-template-version-source-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: TemplateVersionSourceInput
---
