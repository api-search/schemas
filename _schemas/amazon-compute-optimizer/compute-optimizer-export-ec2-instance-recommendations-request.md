---
description: ExportEC2InstanceRecommendationsRequest schema
layout: schema
name: ExportEC2InstanceRecommendationsRequest
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
- description: ''
  name: recommendationPreferences
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-export-ec2-instance-recommendations-request-schema.json
slug: compute-optimizer-export-ec2-instance-recommendations-request
source_filename: compute-optimizer-export-ec2-instance-recommendations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ec2-instance-recommendations-request-schema.json\",\n  \"title\": \"ExportEC2InstanceRecommendationsRequest\",\n  \"description\": \"ExportEC2InstanceRecommendationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p>The IDs of the Amazon Web Services accounts for which to export instance recommendations.</p> <p>If your account is the management account of an organization, use this parameter to specify the member account for which you want to export recommendations.</p> <p>This parameter cannot be specified together with the include member accounts parameter. The parameters are mutually exclusive.</p>\
  \ <p>Recommendations for member accounts are not included in the export if this parameter, or the include member accounts parameter, is omitted.</p> <p>You can specify multiple account IDs per request.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"An array of objects to specify a filter that exports a more specific set of instance recommendations.\"\n        }\n      ]\n    },\n    \"fieldsToExport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportableInstanceFields\"\n        },\n        {\n          \"description\": \"The recommendations data to include in the export file. For more information about the fields that can be exported, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/exporting-recommendations.html#exported-files\\\">Exported files</a> in the <i>Compute Optimizer User Guide</i>.\"\
  \n        }\n      ]\n    },\n    \"s3DestinationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3DestinationConfig\"\n        },\n        {\n          \"description\": \"<p>An object to specify the destination Amazon Simple Storage Service (Amazon S3) bucket name and key prefix for the export job.</p> <p>You must create the destination Amazon S3 bucket for your recommendations export before you create the export job. Compute Optimizer does not create the S3 bucket for you. After you create the S3 bucket, ensure that it has the required permissions policy to allow Compute Optimizer to write the export file to it. If you plan to specify an object prefix when you create the export job, you must include the object prefix in the policy that you add to the S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/create-s3-bucket-policy-for-compute-optimizer.html\\\">Amazon S3 Bucket Policy for Compute Optimizer</a>\
  \ in the <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"fileFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileFormat\"\n        },\n        {\n          \"description\": \"<p>The format of the export file.</p> <p>The only export file format currently supported is <code>Csv</code>.</p>\"\n        }\n      ]\n    },\n    \"includeMemberAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeMemberAccounts\"\n        },\n        {\n          \"description\": \"<p>Indicates whether to include recommendations for resources in all member accounts of the organization if your account is the management account of an organization.</p> <p>The member accounts must also be opted in to Compute Optimizer, and trusted access for Compute Optimizer must be enabled in the organization account. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/security-iam.html#trusted-service-access\\\
  \">Compute Optimizer and Amazon Web Services Organizations trusted access</a> in the <i>Compute Optimizer User Guide</i>.</p> <p>Recommendations for member accounts of the organization are not included in the export file if this parameter is omitted.</p> <p>Recommendations for member accounts are not included in the export if this parameter, or the account IDs parameter, is omitted.</p>\"\n        }\n      ]\n    },\n    \"recommendationPreferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationPreferences\"\n        },\n        {\n          \"description\": \"An object to specify the preferences for the Amazon EC2 instance recommendations to export.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3DestinationConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-export-ec2-instance-recommendations-request-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportEC2InstanceRecommendationsRequest
---
