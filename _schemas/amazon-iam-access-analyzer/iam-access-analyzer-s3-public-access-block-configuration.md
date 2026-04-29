---
description: The <code>PublicAccessBlock</code> configuration to apply to this Amazon S3 bucket. If the proposed configuration is for an existing Amazon S3 bucket and the configuration is not specified, the access preview uses the existing setting. If the proposed configuration is for a new bucket and the configuration is not specified, the access preview uses <code>false</code>. If the proposed configuration is for a new access point or multi-region access point and the access point BPA configuration is not specified, the access preview uses <code>true</code>. For more information, see <a href="https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-s3-bucket-publicaccessblockconfiguration.html">PublicAccessBlockConfiguration</a>.
layout: schema
name: S3PublicAccessBlockConfiguration
properties_list:
- description: ''
  name: ignorePublicAcls
  type: object
- description: ''
  name: restrictPublicBuckets
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-s3-public-access-block-configuration-schema.json
slug: iam-access-analyzer-s3-public-access-block-configuration
source_filename: iam-access-analyzer-s3-public-access-block-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-public-access-block-configuration-schema.json\",\n  \"title\": \"S3PublicAccessBlockConfiguration\",\n  \"description\": \"The <code>PublicAccessBlock</code> configuration to apply to this Amazon S3 bucket. If the proposed configuration is for an existing Amazon S3 bucket and the configuration is not specified, the access preview uses the existing setting. If the proposed configuration is for a new bucket and the configuration is not specified, the access preview uses <code>false</code>. If the proposed configuration is for a new access point or multi-region access point and the access point BPA configuration is not specified, the access preview uses <code>true</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-s3-bucket-publicaccessblockconfiguration.html\\\
  \">PublicAccessBlockConfiguration</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ignorePublicAcls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether Amazon S3 should ignore public ACLs for this bucket and objects in this bucket. \"\n        }\n      ]\n    },\n    \"restrictPublicBuckets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether Amazon S3 should restrict public bucket policies for this bucket. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ignorePublicAcls\",\n    \"restrictPublicBuckets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-public-access-block-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: S3PublicAccessBlockConfiguration
---
