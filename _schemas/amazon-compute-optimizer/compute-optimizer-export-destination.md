---
description: Describes the destination of the recommendations export and metadata files.
layout: schema
name: ExportDestination
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-export-destination-schema.json
slug: compute-optimizer-export-destination
source_filename: compute-optimizer-export-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-destination-schema.json\",\n  \"title\": \"ExportDestination\",\n  \"description\": \"Describes the destination of the recommendations export and metadata files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"description\": \"An object that describes the destination Amazon Simple Storage Service (Amazon S3) bucket name and object keys of a recommendations export file, and its associated metadata file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-destination-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportDestination
---
