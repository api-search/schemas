---
description: ExportEBSVolumeRecommendationsRequest schema
layout: schema
name: ExportEBSVolumeRecommendationsRequest
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
schema_file: json-schema/compute-optimizer-export-ebs-volume-recommendations-request-schema.json
slug: compute-optimizer-export-ebs-volume-recommendations-request
source_filename: compute-optimizer-export-ebs-volume-recommendations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ebs-volume-recommendations-request-schema.json\",\n  \"title\": \"ExportEBSVolumeRecommendationsRequest\",\n  \"description\": \"ExportEBSVolumeRecommendationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p>The IDs of the Amazon Web Services accounts for which to export Amazon EBS volume recommendations.</p> <p>If your account is the management account of an organization, use this parameter to specify the member account for which you want to export recommendations.</p> <p>This parameter cannot be specified together with the include member accounts parameter. The parameters are mutually exclusive.</p>\
  \ <p>Recommendations for member accounts are not included in the export if this parameter, or the include member accounts parameter, is omitted.</p> <p>You can specify multiple account IDs per request.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSFilters\"\n        },\n        {\n          \"description\": \"An array of objects to specify a filter that exports a more specific set of Amazon EBS volume recommendations.\"\n        }\n      ]\n    },\n    \"fieldsToExport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportableVolumeFields\"\n        },\n        {\n          \"description\": \"The recommendations data to include in the export file. For more information about the fields that can be exported, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/exporting-recommendations.html#exported-files\\\">Exported files</a> in the <i>Compute Optimizer\
  \ User Guide</i>.\"\n        }\n      ]\n    },\n    \"s3DestinationConfig\": {\n      \"$ref\": \"#/components/schemas/S3DestinationConfig\"\n    },\n    \"fileFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileFormat\"\n        },\n        {\n          \"description\": \"<p>The format of the export file.</p> <p>The only export file format currently supported is <code>Csv</code>.</p>\"\n        }\n      ]\n    },\n    \"includeMemberAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeMemberAccounts\"\n        },\n        {\n          \"description\": \"<p>Indicates whether to include recommendations for resources in all member accounts of the organization if your account is the management account of an organization.</p> <p>The member accounts must also be opted in to Compute Optimizer, and trusted access for Compute Optimizer must be enabled in the organization account. For more information, see <a href=\\\
  \"https://docs.aws.amazon.com/compute-optimizer/latest/ug/security-iam.html#trusted-service-access\\\">Compute Optimizer and Amazon Web Services Organizations trusted access</a> in the <i>Compute Optimizer User Guide</i>.</p> <p>Recommendations for member accounts of the organization are not included in the export file if this parameter is omitted.</p> <p>This parameter cannot be specified together with the account IDs parameter. The parameters are mutually exclusive.</p> <p>Recommendations for member accounts are not included in the export if this parameter, or the account IDs parameter, is omitted.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3DestinationConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ebs-volume-recommendations-request-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportEBSVolumeRecommendationsRequest
---
