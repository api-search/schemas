---
description: The container for selecting objects from a content event stream.
layout: schema
name: SelectObjectContentEventStream
properties_list:
- description: ''
  name: Records
  type: object
- description: ''
  name: Stats
  type: object
- description: ''
  name: Progress
  type: object
- description: ''
  name: Cont
  type: object
- description: ''
  name: End
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-selectobjectcontenteventstream-schema.json
slug: s3-selectobjectcontenteventstream
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelectObjectContentEventStream\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Records\": {},\n    \"Stats\": {},\n    \"Progress\": {},\n    \"Cont\": {},\n    \"End\": {}\n  },\n  \"description\": \"The container for selecting objects from a content event stream.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-selectobjectcontenteventstream-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: SelectObjectContentEventStream
---
