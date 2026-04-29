---
description: The bucket event for which to send notifications.
layout: schema
name: Event
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-event-schema.json
slug: s3-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Event\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"s3:ReducedRedundancyLostObject\",\n    \"s3:ObjectCreated:*\",\n    \"s3:ObjectCreated:Put\",\n    \"s3:ObjectCreated:Post\",\n    \"s3:ObjectCreated:Copy\",\n    \"s3:ObjectCreated:CompleteMultipartUpload\",\n    \"s3:ObjectRemoved:*\",\n    \"s3:ObjectRemoved:Delete\",\n    \"s3:ObjectRemoved:DeleteMarkerCreated\",\n    \"s3:ObjectRestore:*\",\n    \"s3:ObjectRestore:Post\",\n    \"s3:ObjectRestore:Completed\",\n    \"s3:Replication:*\",\n    \"s3:Replication:OperationFailedReplication\",\n    \"s3:Replication:OperationNotTracked\",\n    \"s3:Replication:OperationMissedThreshold\",\n    \"s3:Replication:OperationReplicatedAfterThreshold\",\n    \"s3:ObjectRestore:Delete\",\n    \"s3:LifecycleTransition\",\n    \"s3:IntelligentTiering\",\n    \"s3:ObjectAcl:Put\",\n    \"s3:LifecycleExpiration:*\",\n    \"s3:LifecycleExpiration:Delete\"\
  ,\n    \"s3:LifecycleExpiration:DeleteMarkerCreated\",\n    \"s3:ObjectTagging:*\",\n    \"s3:ObjectTagging:Put\",\n    \"s3:ObjectTagging:Delete\"\n  ],\n  \"description\": \"The bucket event for which to send notifications.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-event-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Event
---
