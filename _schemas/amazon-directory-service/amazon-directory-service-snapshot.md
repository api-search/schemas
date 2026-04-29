---
description: Describes a directory snapshot.
layout: schema
name: Snapshot
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: SnapshotId
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-snapshot-schema.json
slug: amazon-directory-service-snapshot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-snapshot-schema.json\",\n  \"title\": \"Snapshot\",\n  \"description\": \"Describes a directory snapshot.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier.\"\n        }\n      ]\n    },\n    \"SnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotId\"\n        },\n        {\n          \"description\": \"The snapshot identifier.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotType\"\n        },\n        {\n          \"description\": \"The snapshot type.\"\n\
  \        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotName\"\n        },\n        {\n          \"description\": \"The descriptive name of the snapshot.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotStatus\"\n        },\n        {\n          \"description\": \"The snapshot status.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartTime\"\n        },\n        {\n          \"description\": \"The date and time that the snapshot was taken.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-snapshot-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: Snapshot
---
