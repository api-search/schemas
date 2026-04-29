---
description: Schema representing a Couchbase document with metadata fields used across Server, Sync Gateway, and Capella APIs.
layout: schema
name: Couchbase Document
properties_list:
- description: Unique document identifier within the bucket or collection
  name: _id
  type: string
- description: Revision identifier in Sync Gateway format (generation-digest)
  name: _rev
  type: string
- description: Indicates whether the document is a deletion tombstone
  name: _deleted
  type: boolean
- description: Document expiration time as a Unix timestamp in seconds (0 means no expiry)
  name: _exp
  type: integer
- description: Map of attachment names to attachment metadata
  name: _attachments
  type: object
- description: Sync Gateway metadata (internal, not typically user-facing)
  name: _sync
  type: object
provider_name: Couchbase
provider_slug: couchbase
schema_file: json-schema/couchbase-document-schema.json
slug: couchbase-document
source_filename: couchbase-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://couchbase.com/schemas/couchbase/document.json\",\n  \"title\": \"Couchbase Document\",\n  \"description\": \"Schema representing a Couchbase document with metadata fields used across Server, Sync Gateway, and Capella APIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique document identifier within the bucket or collection\"\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Revision identifier in Sync Gateway format (generation-digest)\",\n      \"pattern\": \"^\\\\d+-[a-f0-9]+$\"\n    },\n    \"_deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the document is a deletion tombstone\",\n      \"default\": false\n    },\n    \"_exp\": {\n      \"type\": \"integer\",\n      \"description\": \"Document expiration time as a Unix timestamp in seconds\
  \ (0 means no expiry)\",\n      \"minimum\": 0\n    },\n    \"_attachments\": {\n      \"type\": \"object\",\n      \"description\": \"Map of attachment names to attachment metadata\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Attachment\"\n      }\n    },\n    \"_sync\": {\n      \"type\": \"object\",\n      \"description\": \"Sync Gateway metadata (internal, not typically user-facing)\",\n      \"properties\": {\n        \"rev\": {\n          \"type\": \"string\",\n          \"description\": \"Current revision\"\n        },\n        \"sequence\": {\n          \"type\": \"integer\",\n          \"description\": \"Sync sequence number\"\n        },\n        \"recent_sequences\": {\n          \"type\": \"array\",\n          \"description\": \"Recent sequence numbers\",\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"history\": {\n          \"type\": \"object\",\n          \"description\": \"Revision history\"\n        },\n\
  \        \"channels\": {\n          \"type\": \"object\",\n          \"description\": \"Channel assignments for this document\"\n        },\n        \"access\": {\n          \"type\": \"object\",\n          \"description\": \"User access grants from this document\"\n        },\n        \"role_access\": {\n          \"type\": \"object\",\n          \"description\": \"Role access grants from this document\"\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"Attachment\": {\n      \"type\": \"object\",\n      \"description\": \"Document attachment metadata\",\n      \"properties\": {\n        \"content_type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the attachment\"\n        },\n        \"digest\": {\n          \"type\": \"string\",\n          \"description\": \"Content digest hash of the attachment\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"description\": \"Size of the attachment\
  \ in bytes\",\n          \"minimum\": 0\n        },\n        \"revpos\": {\n          \"type\": \"integer\",\n          \"description\": \"Revision generation when the attachment was added\",\n          \"minimum\": 1\n        },\n        \"stub\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a stub reference (true) or contains inline data (false)\"\n        },\n        \"data\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded attachment data (only present when not a stub)\",\n          \"contentEncoding\": \"base64\"\n        }\n      },\n      \"required\": [\n        \"content_type\",\n        \"length\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/json-schema/couchbase-document-schema.json
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
title: Couchbase Document
---
