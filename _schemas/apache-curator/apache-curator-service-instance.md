---
description: A service instance registered in ZooKeeper via Apache Curator service discovery.
layout: schema
name: ServiceInstance
properties_list:
- description: Unique identifier for this service instance.
  name: id
  type: string
- description: Service name used to group instances.
  name: name
  type: string
- description: Host address where this service is running.
  name: address
  type: string
- description: Port number this service is listening on.
  name: port
  type: integer
- description: SSL port if the service supports HTTPS.
  name: sslPort
  type:
  - integer
  - 'null'
- description: UTC timestamp (milliseconds) when this instance was registered.
  name: registrationTimeUTC
  type: integer
- description: Service lifecycle type.
  name: serviceType
  type: string
- description: Whether this service instance is currently enabled for discovery.
  name: enabled
  type: boolean
- description: Optional user-defined payload data attached to this service instance.
  name: payload
  type: object
provider_name: Apache Curator
provider_slug: apache-curator
schema_file: json-schema/apache-curator-service-instance-schema.json
slug: apache-curator-service-instance
source_filename: apache-curator-service-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-service-instance-schema.json\",\n  \"title\": \"ServiceInstance\",\n  \"description\": \"A service instance registered in ZooKeeper via Apache Curator service discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this service instance.\",\n      \"example\": \"abc123-def456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name used to group instances.\",\n      \"example\": \"payment-service\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Host address where this service is running.\",\n      \"example\": \"10.1.2.3\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number this service\
  \ is listening on.\",\n      \"example\": 8080\n    },\n    \"sslPort\": {\n      \"type\": [\n        \"integer\",\n        \"null\"\n      ],\n      \"description\": \"SSL port if the service supports HTTPS.\",\n      \"example\": 8443\n    },\n    \"registrationTimeUTC\": {\n      \"type\": \"integer\",\n      \"description\": \"UTC timestamp (milliseconds) when this instance was registered.\",\n      \"example\": 1718153645993\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Service lifecycle type.\",\n      \"enum\": [\n        \"DYNAMIC\",\n        \"STATIC\",\n        \"PERMANENT\"\n      ],\n      \"example\": \"DYNAMIC\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this service instance is currently enabled for discovery.\",\n      \"example\": true\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Optional user-defined payload data attached to this service instance.\"\
  \n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"serviceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-service-instance-schema.json
tags:
- Apache
- Distributed Coordination
- Distributed Systems
- Java
- Maven
- Open Source
- Service Discovery
- ZooKeeper
title: ServiceInstance
---
