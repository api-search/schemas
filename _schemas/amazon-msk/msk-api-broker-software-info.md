---
description: <p>Information about the current software installed on the cluster.</p>
layout: schema
name: BrokerSoftwareInfo
properties_list:
- description: ''
  name: ConfigurationArn
  type: object
- description: ''
  name: ConfigurationRevision
  type: object
- description: ''
  name: KafkaVersion
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-broker-software-info-schema.json
slug: msk-api-broker-software-info
source_filename: msk-api-broker-software-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-software-info-schema.json\",\n  \"title\": \"BrokerSoftwareInfo\",\n  \"description\": \"\\n            <p>Information about the current software installed on the cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurationArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the configuration used for the cluster. This field isn't visible in this preview release.</p>\"\n        }\n      ]\n    },\n    \"ConfigurationRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"configurationRevision\"\n          },\n          \"description\": \"\\n            <p>The revision of the configuration to use. This field isn't visible in this preview release.</p>\"\n        }\n      ]\n    },\n    \"KafkaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaVersion\"\n          },\n          \"description\": \"\\n            <p>The version of Apache Kafka.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-software-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BrokerSoftwareInfo
---
