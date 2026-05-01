---
description: Contains manual snapshot limit information for a directory.
layout: schema
name: SnapshotLimits
properties_list:
- description: ''
  name: ManualSnapshotsLimit
  type: object
- description: ''
  name: ManualSnapshotsCurrentCount
  type: object
- description: ''
  name: ManualSnapshotsLimitReached
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-snapshot-limits-schema.json
slug: amazon-directory-service-snapshot-limits
source_filename: amazon-directory-service-snapshot-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-snapshot-limits-schema.json\",\n  \"title\": \"SnapshotLimits\",\n  \"description\": \"Contains manual snapshot limit information for a directory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManualSnapshotsLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of manual snapshots allowed.\"\n        }\n      ]\n    },\n    \"ManualSnapshotsCurrentCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The current number of manual snapshots of the directory.\"\n        }\n      ]\n    },\n    \"ManualSnapshotsLimitReached\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/ManualSnapshotsLimitReached\"\n        },\n        {\n          \"description\": \"Indicates if the manual snapshot limit has been reached.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-snapshot-limits-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: SnapshotLimits
---
