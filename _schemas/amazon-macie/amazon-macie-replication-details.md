---
description: Provides information about settings that define whether one or more objects in an S3 bucket are replicated to S3 buckets for other Amazon Web Services accounts and, if so, which accounts.
layout: schema
name: ReplicationDetails
properties_list:
- description: ''
  name: replicated
  type: object
- description: ''
  name: replicatedExternally
  type: object
- description: ''
  name: replicationAccounts
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-replication-details-schema.json
slug: amazon-macie-replication-details
source_filename: amazon-macie-replication-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-replication-details-schema.json\",\n  \"title\": \"ReplicationDetails\",\n  \"description\": \"Provides information about settings that define whether one or more objects in an S3 bucket are replicated to S3 buckets for other Amazon Web Services accounts and, if so, which accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"replicated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the bucket is configured to replicate one or more objects to any destination.\"\n        }\n      ]\n    },\n    \"replicatedExternally\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies\
  \ whether the bucket is configured to replicate one or more objects to a bucket for an Amazon Web Services account that isn't part of your Amazon Macie organization. An <i>Amazon Macie organization</i> is a set of Macie accounts that are centrally managed as a group of related accounts through Organizations or by Macie invitation.\"\n        }\n      ]\n    },\n    \"replicationAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of Amazon Web Services account IDs, one for each Amazon Web Services account that owns a bucket that the bucket is configured to replicate one or more objects to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-replication-details-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ReplicationDetails
---
