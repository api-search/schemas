---
description: The set of Amazon Web Services Region that your Incident Manager data will be replicated to and the KMS key used to encrypt the data.
layout: schema
name: ReplicationSet
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdBy
  type: object
- description: ''
  name: createdTime
  type: object
- description: ''
  name: deletionProtected
  type: object
- description: ''
  name: lastModifiedBy
  type: object
- description: ''
  name: lastModifiedTime
  type: object
- description: ''
  name: regionMap
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-replication-set-schema.json
slug: incident-manager-replication-set
source_filename: incident-manager-replication-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-replication-set-schema.json\",\n  \"title\": \"ReplicationSet\",\n  \"description\": \"The set of Amazon Web Services Region that your Incident Manager data will be replicated to and the KMS key used to encrypt the data. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication set.\"\n        }\n      ]\n    },\n    \"createdBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"Details about who created the replication set.\"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the replication set was created.\"\n        }\n      ]\n    },\n    \"deletionProtected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Determines if the replication set deletion protection is enabled or not. If deletion protection is enabled, you can't delete the last Amazon Web Services Region in the replication set. \"\n        }\n      ]\n    },\n    \"lastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"Who last modified the replication set.\"\n        }\n      ]\n    },\n    \"lastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the replication set was last\
  \ updated.\"\n        }\n      ]\n    },\n    \"regionMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionInfoMap\"\n        },\n        {\n          \"description\": \"The map between each Amazon Web Services Region in your replication set and the KMS key that's used to encrypt the data in that Region.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationSetStatus\"\n        },\n        {\n          \"description\": \"The status of the replication set. If the replication set is still pending, you can't use Incident Manager functionality.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdBy\",\n    \"createdTime\",\n    \"deletionProtected\",\n    \"lastModifiedBy\",\n    \"lastModifiedTime\",\n    \"regionMap\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-replication-set-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ReplicationSet
---
