---
description: Describes the public access policies that apply to the S3 bucket.
layout: schema
name: PublicAccess
properties_list:
- description: ''
  name: PermissionConfiguration
  type: object
- description: ''
  name: EffectivePermission
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-public-access-schema.json
slug: guardduty-public-access
source_filename: guardduty-public-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-public-access-schema.json\",\n  \"title\": \"PublicAccess\",\n  \"description\": \"Describes the public access policies that apply to the S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PermissionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"permissionConfiguration\"\n          },\n          \"description\": \"Contains information about how permissions are configured for the S3 bucket.\"\n        }\n      ]\n    },\n    \"EffectivePermission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"effectivePermission\"\n          },\n\
  \          \"description\": \"Describes the effective permission on this bucket after factoring all attached policies.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-public-access-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: PublicAccess
---
