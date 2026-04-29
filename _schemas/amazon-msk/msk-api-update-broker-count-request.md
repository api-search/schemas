---
description: UpdateBrokerCountRequest schema from Amazon MSK API
layout: schema
name: UpdateBrokerCountRequest
properties_list:
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: TargetNumberOfBrokerNodes
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-broker-count-request-schema.json
slug: msk-api-update-broker-count-request
source_filename: msk-api-update-broker-count-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-broker-count-request-schema.json\",\n  \"title\": \"UpdateBrokerCountRequest\",\n  \"description\": \"UpdateBrokerCountRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The version of cluster to update from. A successful operation will then generate a new version.</p>\"\n        }\n      ]\n    },\n    \"TargetNumberOfBrokerNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max15\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetNumberOfBrokerNodes\"\
  \n          },\n          \"description\": \"\\n            <p>The number of broker nodes that you want the cluster to have after this operation completes successfully.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentVersion\",\n    \"TargetNumberOfBrokerNodes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-broker-count-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateBrokerCountRequest
---
