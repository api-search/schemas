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
