---
description: UpdateBrokerTypeRequest schema from Amazon MSK API
layout: schema
name: UpdateBrokerTypeRequest
properties_list:
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: TargetInstanceType
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-broker-type-request-schema.json
slug: msk-api-update-broker-type-request
source_filename: msk-api-update-broker-type-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-broker-type-request-schema.json\",\n  \"title\": \"UpdateBrokerTypeRequest\",\n  \"description\": \"UpdateBrokerTypeRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The cluster version that you want to change. After this operation completes successfully, the cluster will have a new version.</p>\"\n        }\n      ]\n    },\n    \"TargetInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"targetInstanceType\"\n          },\n          \"description\": \"\\n            <p>The Amazon MSK broker type that you want all of the brokers in this cluster to be.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentVersion\",\n    \"TargetInstanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-broker-type-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateBrokerTypeRequest
---
