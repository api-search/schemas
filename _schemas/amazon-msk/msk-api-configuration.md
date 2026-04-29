---
description: <p>Represents an MSK Configuration.</p>
layout: schema
name: Configuration
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: KafkaVersions
  type: object
- description: ''
  name: LatestRevision
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-configuration-schema.json
slug: msk-api-configuration
source_filename: msk-api-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-configuration-schema.json\",\n  \"title\": \"Configuration\",\n  \"description\": \"\\n            <p>Represents an MSK Configuration.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the configuration.</p>\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creationTime\"\n          },\n          \"description\": \"\\n            <p>The time when the configuration\
  \ was created.</p>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"\\n            <p>The description of the configuration.</p>\"\n        }\n      ]\n    },\n    \"KafkaVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaVersions\"\n          },\n          \"description\": \"\\n            <p>An array of the versions of Apache Kafka with which you can use this MSK configuration. You can use this configuration for an MSK cluster only if the Apache Kafka version specified for the cluster appears in this array.</p>\"\n        }\n      ]\n    },\n    \"LatestRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRevision\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"latestRevision\"\n          },\n          \"description\": \"\\n            <p>Latest revision of the configuration.</p>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"\\n            <p>The name of the configuration.</p>\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"\\n            <p>The state of the configuration. The possible states are ACTIVE, DELETING, and DELETE_FAILED. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Description\",\n    \"LatestRevision\",\n    \"CreationTime\"\
  ,\n    \"KafkaVersions\",\n    \"Arn\",\n    \"Name\",\n    \"State\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Configuration
---
