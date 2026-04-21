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
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: SourceSelectionCriteria
---
