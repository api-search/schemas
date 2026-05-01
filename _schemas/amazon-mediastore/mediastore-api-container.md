---
description: This section describes operations that you can perform on an AWS Elemental MediaStore container.
layout: schema
name: Container
properties_list:
- description: ''
  name: Endpoint
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ARN
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: AccessLoggingEnabled
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-container-schema.json
slug: mediastore-api-container
source_filename: mediastore-api-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-container-schema.json\",\n  \"title\": \"Container\",\n  \"description\": \"This section describes operations that you can perform on an AWS Elemental MediaStore container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Endpoint\"\n        },\n        {\n          \"description\": \"The DNS endpoint of the container. Use the endpoint to identify the specific container when sending requests to the data plane. The service assigns this value when the container is created. Once the value has been assigned, it does not change.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n   \
  \       \"description\": \"Unix timestamp.\"\n        }\n      ]\n    },\n    \"ARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the container. The ARN has the following format:</p> <p>arn:aws:&lt;region&gt;:&lt;account that owns this container&gt;:container/&lt;name of container&gt; </p> <p>For example: arn:aws:mediastore:us-west-2:111122223333:container/movies </p>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerStatus\"\n        },\n        {\n          \"description\": \"The status of container creation or deletion. The status is one of the following:\
  \ <code>CREATING</code>, <code>ACTIVE</code>, or <code>DELETING</code>. While the service is creating the container, the status is <code>CREATING</code>. When the endpoint is available, the status changes to <code>ACTIVE</code>.\"\n        }\n      ]\n    },\n    \"AccessLoggingEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerAccessLoggingEnabled\"\n        },\n        {\n          \"description\": \"The state of access logging on the container. This value is <code>false</code> by default, indicating that AWS Elemental MediaStore does not send access logs to Amazon CloudWatch Logs. When you enable access logging on the container, MediaStore changes this value to <code>true</code>, indicating that the service delivers access logs for objects stored in that container to CloudWatch Logs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-container-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Container
---
