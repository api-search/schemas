---
description: AccessPolicySummaries schema
layout: schema
name: AccessPolicySummaries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-access-policy-summaries-schema.json
slug: iot-sitewise-access-policy-summaries
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-access-policy-summaries-schema.json\",\n  \"title\": \"AccessPolicySummaries\",\n  \"description\": \"AccessPolicySummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"id\",\n      \"identity\",\n      \"resource\",\n      \"permission\"\n    ],\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the access policy.\"\n          }\n        ]\n      },\n      \"identity\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Identity\"\n          },\n          {\n            \"description\": \"The identity (an IAM Identity Center user, an IAM Identity Center\
  \ group, or an IAM user).\"\n          }\n        ]\n      },\n      \"resource\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Resource\"\n          },\n          {\n            \"description\": \"The IoT SiteWise Monitor resource (a portal or project).\"\n          }\n        ]\n      },\n      \"permission\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Permission\"\n          },\n          {\n            \"description\": \"The permissions for the access policy. Note that a project <code>ADMINISTRATOR</code> is also known as a project owner.\"\n          }\n        ]\n      },\n      \"creationDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date the access policy was created, in Unix epoch time.\"\n          }\n        ]\n      },\n      \"lastUpdateDate\": {\n        \"allOf\": [\n         \
  \ {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date the access policy was last updated, in Unix epoch time.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains an access policy that defines an identity's access to an IoT SiteWise Monitor resource.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-access-policy-summaries-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AccessPolicySummaries
---
