---
description: ExportEBSVolumeRecommendationsResponse schema
layout: schema
name: ExportEBSVolumeRecommendationsResponse
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: s3Destination
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-export-ebs-volume-recommendations-response-schema.json
slug: compute-optimizer-export-ebs-volume-recommendations-response
source_filename: compute-optimizer-export-ebs-volume-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ebs-volume-recommendations-response-schema.json\",\n  \"title\": \"ExportEBSVolumeRecommendationsResponse\",\n  \"description\": \"ExportEBSVolumeRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"<p>The identification number of the export job.</p> <p>Use the <a>DescribeRecommendationExportJobs</a> action, and specify the job ID to view the status of an export job.</p>\"\n        }\n      ]\n    },\n    \"s3Destination\": {\n      \"$ref\": \"#/components/schemas/S3Destination\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ebs-volume-recommendations-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportEBSVolumeRecommendationsResponse
---
