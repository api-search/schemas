---
description: ValidatePolicyResourceType schema from AWS IAM Access Analyzer API
layout: schema
name: ValidatePolicyResourceType
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-validate-policy-resource-type-schema.json
slug: iam-access-analyzer-validate-policy-resource-type
source_filename: iam-access-analyzer-validate-policy-resource-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-resource-type-schema.json\",\n  \"title\": \"ValidatePolicyResourceType\",\n  \"description\": \"ValidatePolicyResourceType schema from AWS IAM Access Analyzer API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AWS::S3::Bucket\",\n    \"AWS::S3::AccessPoint\",\n    \"AWS::S3::MultiRegionAccessPoint\",\n    \"AWS::S3ObjectLambda::AccessPoint\",\n    \"AWS::IAM::AssumeRolePolicyDocument\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-resource-type-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ValidatePolicyResourceType
---
