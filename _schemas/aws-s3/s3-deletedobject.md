---
description: Information about the deleted object.
layout: schema
name: DeletedObject
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: VersionId
  type: object
- description: ''
  name: DeleteMarker
  type: object
- description: ''
  name: DeleteMarkerVersionId
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-deletedobject-schema.json
slug: s3-deletedobject
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {},\n    \"VersionId\": {},\n    \"DeleteMarker\": {},\n    \"DeleteMarkerVersionId\": {}\n  },\n  \"description\": \"Information about the deleted object.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-deletedobject-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: DeletedObject
---
