---
description: The filter used to describe a set of objects for analyses. A filter must have exactly one prefix, one tag, or one conjunction (AnalyticsAndOperator). If no filter is provided, all objects will be considered in any analysis.
layout: schema
name: AnalyticsFilter
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tag
  type: object
- description: ''
  name: And
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-analyticsfilter-schema.json
slug: s3-analyticsfilter
source_filename: s3-analyticsfilter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnalyticsFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tag\": {},\n    \"And\": {}\n  },\n  \"description\": \"The filter used to describe a set of objects for analyses. A filter must have exactly one prefix, one tag, or one conjunction (AnalyticsAndOperator). If no filter is provided, all objects will be considered in any analysis.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-analyticsfilter-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: AnalyticsFilter
---
