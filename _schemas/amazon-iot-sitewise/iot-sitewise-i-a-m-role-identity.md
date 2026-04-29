---
description: Contains information about an Identity and Access Management role. For more information, see <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html">IAM roles</a> in the <i>IAM User Guide</i>.
layout: schema
name: IAMRoleIdentity
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-i-a-m-role-identity-schema.json
slug: iot-sitewise-i-a-m-role-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-i-a-m-role-identity-schema.json\",\n  \"title\": \"IAMRoleIdentity\",\n  \"description\": \"Contains information about an Identity and Access Management role. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html\\\">IAM roles</a> in the <i>IAM User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html\\\">IAM ARNs</a> in the <i>IAM User Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-i-a-m-role-identity-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: IAMRoleIdentity
---
