---
description: Settings associated with S3 destination
layout: schema
name: S3DestinationSettings
properties_list:
- description: ''
  name: AccessControl
  type: object
- description: ''
  name: Encryption
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-s3-destination-settings-schema.json
slug: mediaconvert-api-s3-destination-settings
source_filename: mediaconvert-api-s3-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-s3-destination-settings-schema.json\",\n  \"title\": \"S3DestinationSettings\",\n  \"description\": \"Settings associated with S3 destination\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3DestinationAccessControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accessControl\"\n          },\n          \"description\": \"Optional. Have MediaConvert automatically apply Amazon S3 access control for the outputs in this output group. When you don't use this setting, S3 automatically applies the default access control list PRIVATE.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3EncryptionSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"Settings for how your job outputs are encrypted as they are uploaded to Amazon S3.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-s3-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: S3DestinationSettings
---
