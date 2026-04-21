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
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicationRule
---
