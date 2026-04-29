---
description: <p>Specifies whether Amazon S3 replicates delete markers. If you specify a <code>Filter</code> in your replication configuration, you must also include a <code>DeleteMarkerReplication</code> element. If your <code>Filter</code> includes a <code>Tag</code> element, the <code>DeleteMarkerReplication</code> <code>Status</code> must be set to Disabled, because Amazon S3 does not support replicating delete markers for tag-based rules. For an example configuration, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-add-config.html#replication-config-min-rule-config">Basic Rule Configuration</a>. </p> <p>For more information about delete marker replication, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/delete-marker-replication.html">Basic Rule Configuration</a>. </p> <note> <p>If you are using an earlier version of the replication configuration, Amazon S3 handles replication of delete markers differently. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-add-config.html#replication-backward-compat-considerations">Backward
  Compatibility</a>.</p> </note>
layout: schema
name: DeleteMarkerReplication
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-deletemarkerreplication-schema.json
slug: s3-deletemarkerreplication
source_filename: s3-deletemarkerreplication-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteMarkerReplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {}\n  },\n  \"description\": \"<p>Specifies whether Amazon S3 replicates delete markers. If you specify a <code>Filter</code> in your replication configuration, you must also include a <code>DeleteMarkerReplication</code> element. If your <code>Filter</code> includes a <code>Tag</code> element, the <code>DeleteMarkerReplication</code> <code>Status</code> must be set to Disabled, because Amazon S3 does not support replicating delete markers for tag-based rules. For an example configuration, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-add-config.html#replication-config-min-rule-config\\\">Basic Rule Configuration</a>. </p> <p>For more information about delete marker replication, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/delete-marker-replication.html\\\
  \">Basic Rule Configuration</a>. </p> <note> <p>If you are using an earlier version of the replication configuration, Amazon S3 handles replication of delete markers differently. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-add-config.html#replication-backward-compat-considerations\\\">Backward Compatibility</a>.</p> </note>\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-deletemarkerreplication-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: DeleteMarkerReplication
---
