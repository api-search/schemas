---
description: JDBC connection configuration for Apache Derby in embedded or client/server mode.
layout: schema
name: ConnectionConfig
properties_list:
- description: Derby deployment mode.
  name: mode
  type: string
- description: Database name or path to create/connect to.
  name: databaseName
  type: string
- description: Network Server hostname (client mode only).
  name: host
  type: string
- description: Network Server port (client mode only).
  name: port
  type: integer
- description: Database user (when authentication is enabled).
  name: user
  type: string
- description: Database password (when authentication is enabled).
  name: password
  type: string
- description: Create the database if it does not exist.
  name: createDatabase
  type: string
- description: Boot password for encrypted databases.
  name: bootPassword
  type: string
- description: Enable data-at-rest encryption for this database.
  name: dataEncryption
  type: boolean
- description: Encryption algorithm for encrypted databases.
  name: encryptionAlgorithm
  type: string
provider_name: Apache Derby
provider_slug: apache-derby
schema_file: json-schema/apache-derby-connection-config-schema.json
slug: apache-derby-connection-config
tags:
- Apache
- Database
- Embedded
- Java
- JDBC
- Open Source
- Relational
- SQL
title: ConnectionConfig
---
