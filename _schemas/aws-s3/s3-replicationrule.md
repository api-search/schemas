---
description: Specifies which Amazon S3 objects to replicate and where to store the replicas.
layout: schema
name: ReplicationRule
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Prefix
  type: object
- description: A filter that identifies the subset of objects to which the replication rule applies. A <code>Filter</code> must specify exactly one <code>Prefix</code>, <code>Tag</code>, or an <code>And</code> child
  name: Filter
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SourceSelectionCriteria
  type: object
- description: ''
  name: ExistingObjectReplication
  type: object
- description: ''
  name: Destination
  type: object
- description: '<p>Specifies whether Amazon S3 replicates delete markers. If you specify a <code>Filter</code> in your replication configuration, you must also include a <code>DeleteMarkerReplication</code> element. '
  name: DeleteMarkerReplication
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicationrule-schema.json
slug: s3-replicationrule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicationRule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {},\n    \"Priority\": {},\n    \"Prefix\": {},\n    \"Filter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Prefix\": {},\n        \"Tag\": {},\n        \"And\": {}\n      },\n      \"description\": \"A filter that identifies the subset of objects to which the replication rule applies. A <code>Filter</code> must specify exactly one <code>Prefix</code>, <code>Tag</code>, or an <code>And</code> child element.\"\n    },\n    \"Status\": {},\n    \"SourceSelectionCriteria\": {},\n    \"ExistingObjectReplication\": {},\n    \"Destination\": {},\n    \"DeleteMarkerReplication\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Status\": {}\n      },\n      \"description\": \"<p>Specifies whether Amazon S3 replicates delete markers. If you specify a <code>Filter</code> in your replication\
  \ configuration, you must also include a <code>DeleteMarkerReplication</code> element. If your <code>Filter</code> includes a <code>Tag</code> element, the <code>DeleteMarkerReplication</code> <code>Status</code> must be set to Disabled, because Amazon S3 does not support replicating delete markers for tag-based rules. For an example configuration, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-add-config.html#replication-config-min-rule-config\\\">Basic Rule Configuration</a>. </p> <p>For more information about delete marker replication, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/delete-marker-replication.html\\\">Basic Rule Configuration</a>. </p> <note> <p>If you are using an earlier version of the replication configuration, Amazon S3 handles replication of delete markers differently. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-add-config.html#replication-backward-compat-considerations\\\
  \">Backward Compatibility</a>.</p> </note>\"\n    }\n  },\n  \"required\": [\n    \"Status\",\n    \"Destination\"\n  ],\n  \"description\": \"Specifies which Amazon S3 objects to replicate and where to store the replicas.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-replicationrule-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicationRule
---
