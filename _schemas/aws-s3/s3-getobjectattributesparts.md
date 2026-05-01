---
description: A collection of parts associated with a multipart upload.
layout: schema
name: GetObjectAttributesParts
properties_list:
- description: ''
  name: TotalPartsCount
  type: object
- description: ''
  name: PartNumberMarker
  type: object
- description: ''
  name: NextPartNumberMarker
  type: object
- description: ''
  name: MaxParts
  type: object
- description: ''
  name: IsTruncated
  type: object
- description: ''
  name: Parts
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-getobjectattributesparts-schema.json
slug: s3-getobjectattributesparts
source_filename: s3-getobjectattributesparts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetObjectAttributesParts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalPartsCount\": {},\n    \"PartNumberMarker\": {},\n    \"NextPartNumberMarker\": {},\n    \"MaxParts\": {},\n    \"IsTruncated\": {},\n    \"Parts\": {}\n  },\n  \"description\": \"A collection of parts associated with a multipart upload.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-getobjectattributesparts-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: GetObjectAttributesParts
---
