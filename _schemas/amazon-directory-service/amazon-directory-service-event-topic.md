---
description: Information about Amazon SNS topic and Directory Service directory associations.
layout: schema
name: EventTopic
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: TopicName
  type: object
- description: ''
  name: TopicArn
  type: object
- description: ''
  name: CreatedDateTime
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-event-topic-schema.json
slug: amazon-directory-service-event-topic
source_filename: amazon-directory-service-event-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-event-topic-schema.json\",\n  \"title\": \"EventTopic\",\n  \"description\": \"Information about Amazon SNS topic and Directory Service directory associations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The Directory ID of an Directory Service directory that will publish status messages to an Amazon SNS topic.\"\n        }\n      ]\n    },\n    \"TopicName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicName\"\n        },\n        {\n          \"description\": \"The name of an Amazon SNS topic the receives status messages from the directory.\"\n        }\n      ]\n\
  \    },\n    \"TopicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicArn\"\n        },\n        {\n          \"description\": \"The Amazon SNS topic ARN (Amazon Resource Name).\"\n        }\n      ]\n    },\n    \"CreatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time of when you associated your directory with the Amazon SNS topic.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicStatus\"\n        },\n        {\n          \"description\": \"The topic registration status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-event-topic-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: EventTopic
---
