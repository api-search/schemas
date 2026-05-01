---
description: TrailPropertiesList schema from AWS IAM Access Analyzer API
layout: schema
name: TrailPropertiesList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-trail-properties-list-schema.json
slug: iam-access-analyzer-trail-properties-list
source_filename: iam-access-analyzer-trail-properties-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-trail-properties-list-schema.json\",\n  \"title\": \"TrailPropertiesList\",\n  \"description\": \"TrailPropertiesList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"cloudTrailArn\"\n    ],\n    \"properties\": {\n      \"cloudTrailArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CloudTrailArn\"\n          },\n          {\n            \"description\": \"Specifies the ARN of the trail. The format of a trail ARN is <code>arn:aws:cloudtrail:us-east-2:123456789012:trail/MyTrail</code>.\"\n          }\n        ]\n      },\n      \"regions\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RegionList\"\n        \
  \  },\n          {\n            \"description\": \"A list of regions to get CloudTrail data from and analyze to generate a policy.\"\n          }\n        ]\n      },\n      \"allRegions\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"Possible values are <code>true</code> or <code>false</code>. If set to <code>true</code>, IAM Access Analyzer retrieves CloudTrail data from all regions to analyze and generate a policy.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains details about the CloudTrail trail being analyzed to generate a policy.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-trail-properties-list-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: TrailPropertiesList
---
