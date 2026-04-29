---
description: Schema representing a Couchbase Server bucket configuration, including type, memory allocation, replication, and eviction settings.
layout: schema
name: Couchbase Bucket Configuration
properties_list:
- description: Name of the bucket
  name: name
  type: string
- description: Type of the bucket determining storage behavior
  name: bucketType
  type: string
- description: RAM quota allocated to the bucket in megabytes
  name: ramQuota
  type: integer
- description: Number of replica copies maintained across the cluster
  name: replicaNumber
  type: integer
- description: Whether to replicate view indexes to replica nodes
  name: replicaIndex
  type: boolean
- description: Strategy for resolving document conflicts during XDCR replication
  name: conflictResolutionType
  type: string
- description: Policy for evicting items from memory when RAM quota is exceeded
  name: evictionPolicy
  type: string
- description: Minimum durability level required for write operations
  name: durabilityMinLevel
  type: string
- description: Maximum time-to-live for documents in seconds (0 means no maximum)
  name: maxTTL
  type: integer
- description: Compression mode for stored documents
  name: compressionMode
  type: string
- description: Whether the flush all operation is enabled on the bucket
  name: flushEnabled
  type: boolean
- description: Storage engine backend for the bucket
  name: storageBackend
  type: string
- description: Scopes defined within the bucket
  name: scopes
  type: array
provider_name: Couchbase
provider_slug: couchbase
schema_file: json-schema/couchbase-bucket-schema.json
slug: couchbase-bucket
source_filename: couchbase-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://couchbase.com/schemas/couchbase/bucket.json\",\n  \"title\": \"Couchbase Bucket Configuration\",\n  \"description\": \"Schema representing a Couchbase Server bucket configuration, including type, memory allocation, replication, and eviction settings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the bucket\",\n      \"maxLength\": 100,\n      \"pattern\": \"^[a-zA-Z0-9._%-]+$\"\n    },\n    \"bucketType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the bucket determining storage behavior\",\n      \"enum\": [\n        \"couchbase\",\n        \"memcached\",\n        \"ephemeral\"\n      ],\n      \"default\": \"couchbase\"\n    },\n    \"ramQuota\": {\n      \"type\": \"integer\",\n      \"description\": \"RAM quota allocated to the bucket in megabytes\"\
  ,\n      \"minimum\": 100\n    },\n    \"replicaNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of replica copies maintained across the cluster\",\n      \"minimum\": 0,\n      \"maximum\": 3,\n      \"default\": 1\n    },\n    \"replicaIndex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to replicate view indexes to replica nodes\",\n      \"default\": false\n    },\n    \"conflictResolutionType\": {\n      \"type\": \"string\",\n      \"description\": \"Strategy for resolving document conflicts during XDCR replication\",\n      \"enum\": [\n        \"seqno\",\n        \"lww\"\n      ],\n      \"default\": \"seqno\"\n    },\n    \"evictionPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Policy for evicting items from memory when RAM quota is exceeded\",\n      \"enum\": [\n        \"valueOnly\",\n        \"fullEviction\",\n        \"noEviction\",\n        \"nruEviction\"\n      ]\n    },\n    \"durabilityMinLevel\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Minimum durability level required for write operations\",\n      \"enum\": [\n        \"none\",\n        \"majority\",\n        \"majorityAndPersistActive\",\n        \"persistToMajority\"\n      ],\n      \"default\": \"none\"\n    },\n    \"maxTTL\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum time-to-live for documents in seconds (0 means no maximum)\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"compressionMode\": {\n      \"type\": \"string\",\n      \"description\": \"Compression mode for stored documents\",\n      \"enum\": [\n        \"off\",\n        \"passive\",\n        \"active\"\n      ],\n      \"default\": \"passive\"\n    },\n    \"flushEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the flush all operation is enabled on the bucket\",\n      \"default\": false\n    },\n    \"storageBackend\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Storage engine backend for the bucket\",\n      \"enum\": [\n        \"couchstore\",\n        \"magma\"\n      ],\n      \"default\": \"couchstore\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"description\": \"Scopes defined within the bucket\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Scope\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Scope\": {\n      \"type\": \"object\",\n      \"description\": \"A scope within a bucket that contains collections\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the scope\"\n        },\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the scope\"\n        },\n        \"collections\": {\n          \"type\": \"array\",\n          \"description\": \"Collections within the scope\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Collection\"\n\
  \          }\n        }\n      }\n    },\n    \"Collection\": {\n      \"type\": \"object\",\n      \"description\": \"A collection within a scope\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the collection\"\n        },\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the collection\"\n        },\n        \"maxTTL\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum TTL for documents in the collection in seconds\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/json-schema/couchbase-bucket-schema.json
tags:
- Analytics
- App Services
- Backup
- Capella
- Cloud
- Database
- DBaaS
- Eventing
- Full-Text Search
- Gateway
- JSON
- Mobile
- NoSQL
- Replication
- SQL++
- Sync
- Vector Search
- XDCR
title: Couchbase Bucket Configuration
---
