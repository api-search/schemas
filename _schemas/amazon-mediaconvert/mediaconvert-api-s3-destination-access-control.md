---
description: Optional. Have MediaConvert automatically apply Amazon S3 access control for the outputs in this output group. When you don't use this setting, S3 automatically applies the default access control list PRIVATE.
layout: schema
name: S3DestinationAccessControl
properties_list:
- description: ''
  name: CannedAcl
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-s3-destination-access-control-schema.json
slug: mediaconvert-api-s3-destination-access-control
source_filename: mediaconvert-api-s3-destination-access-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-s3-destination-access-control-schema.json\",\n  \"title\": \"S3DestinationAccessControl\",\n  \"description\": \"Optional. Have MediaConvert automatically apply Amazon S3 access control for the outputs in this output group. When you don't use this setting, S3 automatically applies the default access control list PRIVATE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CannedAcl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ObjectCannedAcl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cannedAcl\"\n          },\n          \"description\": \"Choose an Amazon S3 canned ACL for MediaConvert to apply to this output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-s3-destination-access-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: S3DestinationAccessControl
---
