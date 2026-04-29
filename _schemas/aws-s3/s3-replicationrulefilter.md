---
description: A filter that identifies the subset of objects to which the replication rule applies. A <code>Filter</code> must specify exactly one <code>Prefix</code>, <code>Tag</code>, or an <code>And</code> child element.
layout: schema
name: ReplicationRuleFilter
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tag
  type: object
- description: ''
  name: And
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicationrulefilter-schema.json
slug: s3-replicationrulefilter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicationRuleFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tag\": {},\n    \"And\": {}\n  },\n  \"description\": \"A filter that identifies the subset of objects to which the replication rule applies. A <code>Filter</code> must specify exactly one <code>Prefix</code>, <code>Tag</code>, or an <code>And</code> child element.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-replicationrulefilter-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicationRuleFilter
---
