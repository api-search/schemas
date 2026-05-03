---
description: JSON Schema for Vert.x verticle deployment options used when deploying verticles programmatically or via configuration.
layout: schema
name: Vert.x Verticle Deployment Descriptor
properties_list:
- description: The main verticle class name or script path to deploy.
  name: main
  type: string
- description: Deployment options for the verticle.
  name: options
  type: object
provider_name: Vert.x
provider_slug: vert-x
schema_file: json-schema/vertx-deployment-descriptor.json
slug: vertx-deployment-descriptor
source_filename: vertx-deployment-descriptor.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vert-x/json-schema/vertx-deployment-descriptor.json\",\n  \"title\": \"Vert.x Verticle Deployment Descriptor\",\n  \"description\": \"JSON Schema for Vert.x verticle deployment options used when deploying verticles programmatically or via configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"main\": {\n      \"type\": \"string\",\n      \"description\": \"The main verticle class name or script path to deploy.\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Deployment options for the verticle.\",\n      \"properties\": {\n        \"instances\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of verticle instances to deploy.\",\n          \"default\": 1,\n          \"minimum\": 1\n        },\n        \"worker\": {\n          \"type\": \"boolean\",\n          \"description\": \"Deploy\
  \ as a worker verticle.\",\n          \"default\": false\n        },\n        \"multiThreaded\": {\n          \"type\": \"boolean\",\n          \"description\": \"Deploy as a multi-threaded worker verticle.\",\n          \"default\": false\n        },\n        \"ha\": {\n          \"type\": \"boolean\",\n          \"description\": \"Deploy with high availability.\",\n          \"default\": false\n        },\n        \"isolationGroup\": {\n          \"type\": \"string\",\n          \"description\": \"Isolation group for the verticle classloader.\"\n        },\n        \"isolatedClasses\": {\n          \"type\": \"array\",\n          \"description\": \"List of class name patterns to isolate.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"extraClasspath\": {\n          \"type\": \"array\",\n          \"description\": \"Extra classpath entries for the verticle.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n    \
  \    },\n        \"config\": {\n          \"type\": \"object\",\n          \"description\": \"JSON configuration passed to the verticle.\",\n          \"additionalProperties\": true\n        },\n        \"workerPoolName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the worker pool to use.\"\n        },\n        \"workerPoolSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Size of the worker pool.\",\n          \"minimum\": 1\n        },\n        \"maxWorkerExecuteTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Max worker execute time in nanoseconds.\"\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"main\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vert-x/refs/heads/main/json-schema/vertx-deployment-descriptor.json
tags:
- Event-Driven
- Frameworks
- Java
- JVM
- Microservices
- Polyglot
- Reactive
title: Vert.x Verticle Deployment Descriptor
---
