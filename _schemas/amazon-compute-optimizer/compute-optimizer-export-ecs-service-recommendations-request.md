---
description: ExportECSServiceRecommendationsRequest schema
layout: schema
name: ExportECSServiceRecommendationsRequest
properties_list:
- description: ''
  name: accountIds
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: fieldsToExport
  type: object
- description: ''
  name: s3DestinationConfig
  type: object
- description: ''
  name: fileFormat
  type: object
- description: ''
  name: includeMemberAccounts
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-export-ecs-service-recommendations-request-schema.json
slug: compute-optimizer-export-ecs-service-recommendations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ecs-service-recommendations-request-schema.json\",\n  \"title\": \"ExportECSServiceRecommendationsRequest\",\n  \"description\": \"ExportECSServiceRecommendationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p> The Amazon Web Services account IDs for the export Amazon ECS service recommendations. </p> <p>If your account is the management account or the delegated administrator of an organization, use this parameter to specify the member account you want to export recommendations to.</p> <p>This parameter can't be specified together with the include member accounts parameter. The parameters\
  \ are mutually exclusive.</p> <p>If this parameter or the include member accounts parameter is omitted, the recommendations for member accounts aren't included in the export.</p> <p>You can specify multiple account IDs per request.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendationFilters\"\n        },\n        {\n          \"description\": \" An array of objects to specify a filter that exports a more specific set of Amazon ECS service recommendations. \"\n        }\n      ]\n    },\n    \"fieldsToExport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportableECSServiceFields\"\n        },\n        {\n          \"description\": \"The recommendations data to include in the export file. For more information about the fields that can be exported, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/exporting-recommendations.html#exported-files\\\
  \">Exported files</a> in the <i>Compute Optimizer User Guide</i>.\"\n        }\n      ]\n    },\n    \"s3DestinationConfig\": {\n      \"$ref\": \"#/components/schemas/S3DestinationConfig\"\n    },\n    \"fileFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileFormat\"\n        },\n        {\n          \"description\": \"<p> The format of the export file. </p> <p>The CSV file is the only export file format currently supported.</p>\"\n        }\n      ]\n    },\n    \"includeMemberAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeMemberAccounts\"\n        },\n        {\n          \"description\": \"<p>If your account is the management account or the delegated administrator of an organization, this parameter indicates whether to include recommendations for resources in all member accounts of the organization.</p> <p>The member accounts must also be opted in to Compute Optimizer, and trusted access for Compute\
  \ Optimizer must be enabled in the organization account. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/security-iam.html#trusted-service-access\\\">Compute Optimizer and Amazon Web Services Organizations trusted access</a> in the <i>Compute Optimizer User Guide</i>.</p> <p>If this parameter is omitted, recommendations for member accounts of the organization aren't included in the export file.</p> <p>If this parameter or the account ID parameter is omitted, recommendations for member accounts aren't included in the export.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3DestinationConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ecs-service-recommendations-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportECSServiceRecommendationsRequest
---
