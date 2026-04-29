---
description: Describes a Fleet Advisor collector.
layout: schema
name: CollectorResponse
properties_list:
- description: ''
  name: CollectorReferencedId
  type: object
- description: ''
  name: CollectorName
  type: object
- description: ''
  name: CollectorVersion
  type: object
- description: ''
  name: VersionStatus
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: S3BucketName
  type: object
- description: ''
  name: ServiceAccessRoleArn
  type: object
- description: ''
  name: CollectorHealthCheck
  type: object
- description: ''
  name: LastDataReceived
  type: object
- description: ''
  name: RegisteredDate
  type: object
- description: ''
  name: CreatedDate
  type: object
- description: ''
  name: ModifiedDate
  type: object
- description: ''
  name: InventoryData
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-collector-response-schema.json
slug: amazon-dms-collector-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-collector-response-schema.json\",\n  \"title\": \"CollectorResponse\",\n  \"description\": \"Describes a Fleet Advisor collector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CollectorReferencedId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reference ID of the Fleet Advisor collector.\"\n        }\n      ]\n    },\n    \"CollectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the Fleet Advisor collector .\"\n        }\n      ]\n    },\n    \"CollectorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n     \
  \     \"description\": \"The version of your Fleet Advisor collector, in semantic versioning format, for example <code>1.0.2</code> \"\n        }\n      ]\n    },\n    \"VersionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionStatus\"\n        },\n        {\n          \"description\": \"Whether the collector version is up to date.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A summary description of the Fleet Advisor collector.\"\n        }\n      ]\n    },\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket that the Fleet Advisor collector uses to store inventory metadata.\"\n        }\n      ]\n    },\n    \"ServiceAccessRoleArn\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The IAM role that grants permissions to access the specified Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"CollectorHealthCheck\": {\n      \"$ref\": \"#/components/schemas/CollectorHealthCheck\"\n    },\n    \"LastDataReceived\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The timestamp of the last time the collector received data, in the following format: <code>2022-01-24T19:04:02.596113Z</code> \"\n        }\n      ]\n    },\n    \"RegisteredDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The timestamp when DMS registered the collector, in the following format: <code>2022-01-24T19:04:02.596113Z</code> \"\n        }\n      ]\n    },\n    \"CreatedDate\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The timestamp when you created the collector, in the following format: <code>2022-01-24T19:04:02.596113Z</code> \"\n        }\n      ]\n    },\n    \"ModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The timestamp when DMS last modified the collector, in the following format: <code>2022-01-24T19:04:02.596113Z</code> \"\n        }\n      ]\n    },\n    \"InventoryData\": {\n      \"$ref\": \"#/components/schemas/InventoryData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-collector-response-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: CollectorResponse
---
