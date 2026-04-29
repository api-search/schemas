---
description: <p>The settings for encrypting data in transit.</p>
layout: schema
name: EncryptionInTransit
properties_list:
- description: ''
  name: ClientBroker
  type: object
- description: ''
  name: InCluster
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-encryption-in-transit-schema.json
slug: msk-api-encryption-in-transit
source_filename: msk-api-encryption-in-transit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-encryption-in-transit-schema.json\",\n  \"title\": \"EncryptionInTransit\",\n  \"description\": \"\\n            <p>The settings for encrypting data in transit.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientBroker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientBroker\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientBroker\"\n          },\n          \"description\": \"\\n            <p>Indicates the encryption setting for data in transit between clients and brokers. The following are the possible values.</p>\\n            <p>\\n               TLS means that client-broker communication is enabled with TLS only.</p>\\n            <p>\\n               TLS_PLAINTEXT means that client-broker communication is enabled for\
  \ both TLS-encrypted, as well as plaintext data.</p>\\n            <p>\\n               PLAINTEXT means that client-broker communication is enabled in plaintext only.</p>\\n            <p>The default value is TLS_PLAINTEXT.</p>\"\n        }\n      ]\n    },\n    \"InCluster\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inCluster\"\n          },\n          \"description\": \"\\n            <p>When set to true, it indicates that data communication among the broker nodes of the cluster is encrypted. When set to false, the communication happens in plaintext.</p>\\n            <p>The default value is true.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-encryption-in-transit-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: EncryptionInTransit
---
