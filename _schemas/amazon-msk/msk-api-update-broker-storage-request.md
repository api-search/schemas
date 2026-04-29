---
description: UpdateBrokerStorageRequest schema from Amazon MSK API
layout: schema
name: UpdateBrokerStorageRequest
properties_list:
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: TargetBrokerEBSVolumeInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-broker-storage-request-schema.json
slug: msk-api-update-broker-storage-request
source_filename: msk-api-update-broker-storage-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-broker-storage-request-schema.json\",\n  \"title\": \"UpdateBrokerStorageRequest\",\n  \"description\": \"UpdateBrokerStorageRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The version of cluster to update from. A successful operation will then generate a new version.</p>\"\n        }\n      ]\n    },\n    \"TargetBrokerEBSVolumeInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBrokerEBSVolumeInfo\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"targetBrokerEBSVolumeInfo\"\n          },\n          \"description\": \"\\n            <p>Describes the target volume size and the ID of the broker to apply the update to.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetBrokerEBSVolumeInfo\",\n    \"CurrentVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-broker-storage-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateBrokerStorageRequest
---
