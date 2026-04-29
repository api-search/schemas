---
description: Contains counts of vulnerability findings from image scans that run when you create new Image Builder images, or build new versions of existing images. The vulnerability counts are grouped by severity level. The counts are aggregated across resources to create the final tally for the account that owns them.
layout: schema
name: AccountAggregation
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-account-aggregation-schema.json
slug: ec2-image-builder-account-aggregation
source_filename: ec2-image-builder-account-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-account-aggregation-schema.json\",\n  \"title\": \"AccountAggregation\",\n  \"description\": \"Contains counts of vulnerability findings from image scans that run when you create new Image Builder images, or build new versions of existing images. The vulnerability counts are grouped by severity level. The counts are aggregated across resources to create the final tally for the account that owns them.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Identifies the account that owns the aggregated resource findings.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"Counts by severity level for medium severity and higher level findings, plus a total for all of the findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-account-aggregation-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: AccountAggregation
---
