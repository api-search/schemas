---
description: <p>Describes a recommendation export job.</p> <p>Use the <a>DescribeRecommendationExportJobs</a> action to view your recommendation export jobs.</p> <p>Use the <a>ExportAutoScalingGroupRecommendations</a> or <a>ExportEC2InstanceRecommendations</a> actions to request an export of your recommendations.</p>
layout: schema
name: RecommendationExportJob
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: creationTimestamp
  type: object
- description: ''
  name: lastUpdatedTimestamp
  type: object
- description: ''
  name: failureReason
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-recommendation-export-job-schema.json
slug: compute-optimizer-recommendation-export-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-export-job-schema.json\",\n  \"title\": \"RecommendationExportJob\",\n  \"description\": \"<p>Describes a recommendation export job.</p> <p>Use the <a>DescribeRecommendationExportJobs</a> action to view your recommendation export jobs.</p> <p>Use the <a>ExportAutoScalingGroupRecommendations</a> or <a>ExportEC2InstanceRecommendations</a> actions to request an export of your recommendations.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identification number of the export job.\"\n        }\n      ]\n    },\n    \"destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportDestination\"\
  \n        },\n        {\n          \"description\": \"An object that describes the destination of the export file.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The resource type of the exported recommendations.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The status of the export job.\"\n        }\n      ]\n    },\n    \"creationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationTimestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the export job was created.\"\n        }\n      ]\n    },\n    \"lastUpdatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTimestamp\"\
  \n        },\n        {\n          \"description\": \"The timestamp of when the export job was last updated.\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureReason\"\n        },\n        {\n          \"description\": \"The reason for an export job failure.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-export-job-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: RecommendationExportJob
---
