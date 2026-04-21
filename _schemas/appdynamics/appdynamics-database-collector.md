---
description: Schema representing an AppDynamics Database Visibility collector configuration for monitoring database instances.
layout: schema
name: AppDynamics Database Collector
properties_list:
- description: The internal configuration ID for the database collector.
  name: id
  type: integer
- description: The display name for the database collector.
  name: name
  type: string
- description: The type of database being monitored.
  name: type
  type: string
- description: The hostname or IP address of the database server.
  name: hostname
  type: string
- description: The port number for the database connection.
  name: port
  type: integer
- description: The username for authenticating with the database.
  name: username
  type: string
- description: The password for authenticating with the database. Only used in create and update requests.
  name: password
  type: string
- description: The name of the specific database to monitor.
  name: databaseName
  type: string
- description: Whether the database collector is enabled and actively monitoring.
  name: enabled
  type: boolean
- description: The name of the Database Agent responsible for this collector.
  name: agentName
  type: string
- description: List of schema names to exclude from monitoring.
  name: excludedSchemas
  type: array
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-database-collector-schema.json
slug: appdynamics-database-collector
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Database Collector
---
