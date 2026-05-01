---
description: A Cloud Storage bucket resource representing a container for objects stored in Google Cloud Storage.
layout: schema
name: Google Cloud Storage Bucket
properties_list:
- description: The kind of item this is. Always storage#bucket.
  name: kind
  type: string
- description: The ID of the bucket.
  name: id
  type: string
- description: The URI of this bucket.
  name: selfLink
  type: string
- description: The name of the bucket.
  name: name
  type: string
- description: The project number of the project the bucket belongs to.
  name: projectNumber
  type: string
- description: The creation time of the bucket in RFC 3339 format.
  name: timeCreated
  type: string
- description: The modification time of the bucket in RFC 3339 format.
  name: updated
  type: string
- description: The location of the bucket (e.g., US, EU, us-central1).
  name: location
  type: string
- description: The type of the bucket location.
  name: locationType
  type: string
- description: The default storage class of the bucket.
  name: storageClass
  type: string
- description: ''
  name: versioning
  type: object
- description: User-provided labels in key/value pairs.
  name: labels
  type: object
- description: The bucket's lifecycle configuration.
  name: lifecycle
  type: object
- description: ''
  name: encryption
  type: object
- description: ''
  name: iamConfiguration
  type: object
- description: The metadata generation of this bucket.
  name: metageneration
  type: string
- description: HTTP 1.1 Entity tag for the bucket.
  name: etag
  type: string
provider_name: Google Cloud Storage
provider_slug: google-cloud-storage
schema_file: json-schema/bucket-schema.json
slug: bucket
source_filename: bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-storage/refs/heads/main/json-schema/bucket-schema.json\",\n  \"title\": \"Google Cloud Storage Bucket\",\n  \"description\": \"A Cloud Storage bucket resource representing a container for objects stored in Google Cloud Storage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"storage#bucket\",\n      \"description\": \"The kind of item this is. Always storage#bucket.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the bucket.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URI of this bucket.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\",\n      \"minLength\": 3,\n      \"maxLength\": 63,\n      \"\
  pattern\": \"^[a-z0-9][a-z0-9._-]*[a-z0-9]$\"\n    },\n    \"projectNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The project number of the project the bucket belongs to.\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the bucket in RFC 3339 format.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The modification time of the bucket in RFC 3339 format.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the bucket (e.g., US, EU, us-central1).\"\n    },\n    \"locationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"region\", \"dual-region\", \"multi-region\"],\n      \"description\": \"The type of the bucket location.\"\n    },\n    \"storageClass\": {\n      \"type\": \"string\",\n      \"enum\": [\"STANDARD\", \"NEARLINE\", \"COLDLINE\", \"\
  ARCHIVE\"],\n      \"description\": \"The default storage class of the bucket.\"\n    },\n    \"versioning\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether versioning is enabled for the bucket.\"\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-provided labels in key/value pairs.\"\n    },\n    \"lifecycle\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"rule\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"action\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"enum\": [\"Delete\", \"SetStorageClass\", \"AbortIncompleteMultipartUpload\"\
  ]\n                  },\n                  \"storageClass\": {\n                    \"type\": \"string\"\n                  }\n                },\n                \"required\": [\"type\"]\n              },\n              \"condition\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"age\": { \"type\": \"integer\" },\n                  \"isLive\": { \"type\": \"boolean\" },\n                  \"numNewerVersions\": { \"type\": \"integer\" },\n                  \"createdBefore\": { \"type\": \"string\", \"format\": \"date\" },\n                  \"matchesStorageClass\": {\n                    \"type\": \"array\",\n                    \"items\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            }\n          }\n        }\n      },\n      \"description\": \"The bucket's lifecycle configuration.\"\n    },\n    \"encryption\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"defaultKmsKeyName\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Cloud KMS key name for default bucket encryption.\"\n        }\n      }\n    },\n    \"iamConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uniformBucketLevelAccess\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": { \"type\": \"boolean\" },\n            \"lockedTime\": { \"type\": \"string\", \"format\": \"date-time\" }\n          }\n        },\n        \"publicAccessPrevention\": {\n          \"type\": \"string\",\n          \"enum\": [\"inherited\", \"enforced\"]\n        }\n      }\n    },\n    \"metageneration\": {\n      \"type\": \"string\",\n      \"description\": \"The metadata generation of this bucket.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP 1.1 Entity tag for the bucket.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-storage/refs/heads/main/json-schema/bucket-schema.json
tags:
- Buckets
- Cloud
- Google Cloud
- Objects
- Storage
title: Google Cloud Storage Bucket
---
