---
description: Represents a Pub/Sub topic, which is a named resource to which messages are sent by publishers.
layout: schema
name: Google Cloud Pub/Sub Topic
properties_list:
- description: The name of the topic in the format projects/{project}/topics/{topic}.
  name: name
  type: string
- description: User labels for the topic.
  name: labels
  type: object
- description: Policy constraining the set of Google Cloud regions where messages published to the topic may be stored.
  name: messageStoragePolicy
  type: object
- description: The resource name of the Cloud KMS CryptoKey used to protect access to messages published on this topic.
  name: kmsKeyName
  type: string
- description: Settings for validating messages published against a schema.
  name: schemaSettings
  type: object
- description: Reserved for future use.
  name: satisfiesPzs
  type: boolean
- description: How long to retain unacknowledged messages in the topic's backlog, from the moment a message is published.
  name: messageRetentionDuration
  type: string
provider_name: Google Cloud Pub/Sub
provider_slug: google-cloud-pubsub
schema_file: json-schema/google-cloud-pubsub-topic-schema.json
slug: google-cloud-pubsub-topic
source_filename: google-cloud-pubsub-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-pubsub/refs/heads/main/json-schema/google-cloud-pubsub-topic-schema.json\",\n  \"title\": \"Google Cloud Pub/Sub Topic\",\n  \"description\": \"Represents a Pub/Sub topic, which is a named resource to which messages are sent by publishers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the topic in the format projects/{project}/topics/{topic}.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"User labels for the topic.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"messageStoragePolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Policy constraining the set of Google Cloud regions where messages published to the topic may be stored.\",\n      \"properties\"\
  : {\n        \"allowedPersistenceRegions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A list of IDs of Google Cloud regions where messages published to the topic may be persisted.\"\n        }\n      }\n    },\n    \"kmsKeyName\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the Cloud KMS CryptoKey used to protect access to messages published on this topic.\"\n    },\n    \"schemaSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for validating messages published against a schema.\",\n      \"properties\": {\n        \"schema\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the schema that messages published should be validated against.\"\n        },\n        \"encoding\": {\n          \"type\": \"string\",\n          \"enum\": [\"ENCODING_UNSPECIFIED\", \"JSON\", \"BINARY\"],\n          \"description\"\
  : \"The encoding of messages validated against the schema.\"\n        },\n        \"firstRevisionId\": {\n          \"type\": \"string\"\n        },\n        \"lastRevisionId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"satisfiesPzs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Reserved for future use.\"\n    },\n    \"messageRetentionDuration\": {\n      \"type\": \"string\",\n      \"description\": \"How long to retain unacknowledged messages in the topic's backlog, from the moment a message is published.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-pubsub/refs/heads/main/json-schema/google-cloud-pubsub-topic-schema.json
tags:
- Event-Driven
- Google Cloud
- Messaging
- Pub/Sub
title: Google Cloud Pub/Sub Topic
---
