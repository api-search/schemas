---
description: A container that describes additional filters for identifying the source objects that you want to replicate. You can choose to enable or disable the replication of these objects. Currently, Amazon S3 supports only the filter that you can specify for objects created with server-side encryption using a customer managed key stored in Amazon Web Services Key Management Service (SSE-KMS).
layout: schema
name: SourceSelectionCriteria
properties_list:
- description: ''
  name: SseKmsEncryptedObjects
  type: object
- description: ''
  name: ReplicaModifications
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-sourceselectioncriteria-schema.json
slug: s3-sourceselectioncriteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SourceSelectionCriteria\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SseKmsEncryptedObjects\": {},\n    \"ReplicaModifications\": {}\n  },\n  \"description\": \"A container that describes additional filters for identifying the source objects that you want to replicate. You can choose to enable or disable the replication of these objects. Currently, Amazon S3 supports only the filter that you can specify for objects created with server-side encryption using a customer managed key stored in Amazon Web Services Key Management Service (SSE-KMS).\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-sourceselectioncriteria-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: SourceSelectionCriteria
---
