---
description: Contains information about an Identity and Access Management user.
layout: schema
name: IAMUserIdentity
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-i-a-m-user-identity-schema.json
slug: iot-sitewise-i-a-m-user-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-i-a-m-user-identity-schema.json\",\n  \"title\": \"IAMUserIdentity\",\n  \"description\": \"Contains information about an Identity and Access Management user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The ARN of the IAM user. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html\\\">IAM ARNs</a> in the <i>IAM User Guide</i>.</p> <note> <p>If you delete the IAM user, access policies that contain this identity include an empty <code>arn</code>. You can delete the access policy for the IAM user that no longer exists.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-i-a-m-user-identity-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: IAMUserIdentity
---
