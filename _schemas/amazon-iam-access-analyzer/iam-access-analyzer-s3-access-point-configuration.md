---
description: The configuration for an Amazon S3 access point or multi-region access point for the bucket. You can propose up to 10 access points or multi-region access points per bucket. If the proposed Amazon S3 access point configuration is for an existing bucket, the access preview uses the proposed access point configuration in place of the existing access points. To propose an access point without a policy, you can provide an empty string as the access point policy. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/creating-access-points.html">Creating access points</a>. For more information about access point policy limits, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/access-points-restrictions-limitations.html">Access points restrictions and limitations</a>.
layout: schema
name: S3AccessPointConfiguration
properties_list:
- description: ''
  name: accessPointPolicy
  type: object
- description: ''
  name: publicAccessBlock
  type: object
- description: ''
  name: networkOrigin
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-s3-access-point-configuration-schema.json
slug: iam-access-analyzer-s3-access-point-configuration
source_filename: iam-access-analyzer-s3-access-point-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-access-point-configuration-schema.json\",\n  \"title\": \"S3AccessPointConfiguration\",\n  \"description\": \"The configuration for an Amazon S3 access point or multi-region access point for the bucket. You can propose up to 10 access points or multi-region access points per bucket. If the proposed Amazon S3 access point configuration is for an existing bucket, the access preview uses the proposed access point configuration in place of the existing access points. To propose an access point without a policy, you can provide an empty string as the access point policy. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/creating-access-points.html\\\">Creating access points</a>. For more information about access point policy limits, see <a\
  \ href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-points-restrictions-limitations.html\\\">Access points restrictions and limitations</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPointPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPointPolicy\"\n        },\n        {\n          \"description\": \"The access point or multi-region access point policy.\"\n        }\n      ]\n    },\n    \"publicAccessBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3PublicAccessBlockConfiguration\"\n        },\n        {\n          \"description\": \"The proposed <code>S3PublicAccessBlock</code> configuration to apply to this Amazon S3 access point or multi-region access point.\"\n        }\n      ]\n    },\n    \"networkOrigin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkOriginConfiguration\"\n        },\n        {\n          \"description\":\
  \ \"The proposed <code>Internet</code> and <code>VpcConfiguration</code> to apply to this Amazon S3 access point. <code>VpcConfiguration</code> does not apply to multi-region access points. If the access preview is for a new resource and neither is specified, the access preview uses <code>Internet</code> for the network origin. If the access preview is for an existing resource and neither is specified, the access preview uses the exiting network origin.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-access-point-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: S3AccessPointConfiguration
---
