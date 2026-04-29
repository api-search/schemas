---
description: <p>Contains an identity that can access an IoT SiteWise Monitor resource.</p> <note> <p>Currently, you can't use Amazon Web Services APIs to retrieve IAM Identity Center identity IDs. You can find the IAM Identity Center identity IDs in the URL of user and group pages in the <a href="https://console.aws.amazon.com/singlesignon">IAM Identity Center console</a>.</p> </note>
layout: schema
name: Identity
properties_list:
- description: ''
  name: user
  type: object
- description: ''
  name: group
  type: object
- description: ''
  name: iamUser
  type: object
- description: ''
  name: iamRole
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-identity-schema.json
slug: iot-sitewise-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-identity-schema.json\",\n  \"title\": \"Identity\",\n  \"description\": \"<p>Contains an identity that can access an IoT SiteWise Monitor resource.</p> <note> <p>Currently, you can't use Amazon Web Services APIs to retrieve IAM Identity Center identity IDs. You can find the IAM Identity Center identity IDs in the URL of user and group pages in the <a href=\\\"https://console.aws.amazon.com/singlesignon\\\">IAM Identity Center console</a>.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdentity\"\n        },\n        {\n          \"description\": \"An IAM Identity Center user identity.\"\n        }\n      ]\n    },\n    \"group\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/GroupIdentity\"\n        },\n        {\n          \"description\": \"An IAM Identity Center group identity.\"\n        }\n      ]\n    },\n    \"iamUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IAMUserIdentity\"\n        },\n        {\n          \"description\": \"An IAM user identity.\"\n        }\n      ]\n    },\n    \"iamRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IAMRoleIdentity\"\n        },\n        {\n          \"description\": \"An IAM role identity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-identity-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Identity
---
