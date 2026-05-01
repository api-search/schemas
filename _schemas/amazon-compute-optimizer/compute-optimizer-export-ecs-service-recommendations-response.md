---
description: ExportECSServiceRecommendationsResponse schema
layout: schema
name: ExportECSServiceRecommendationsResponse
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: s3Destination
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-export-ecs-service-recommendations-response-schema.json
slug: compute-optimizer-export-ecs-service-recommendations-response
source_filename: compute-optimizer-export-ecs-service-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ecs-service-recommendations-response-schema.json\",\n  \"title\": \"ExportECSServiceRecommendationsResponse\",\n  \"description\": \"ExportECSServiceRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"<p> The identification number of the export job. </p> <p>To view the status of an export job, use the <a>DescribeRecommendationExportJobs</a> action and specify the job ID. </p>\"\n        }\n      ]\n    },\n    \"s3Destination\": {\n      \"$ref\": \"#/components/schemas/S3Destination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ecs-service-recommendations-response-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportECSServiceRecommendationsResponse
---
