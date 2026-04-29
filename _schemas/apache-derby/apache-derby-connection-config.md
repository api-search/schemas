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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-derby/refs/heads/main/json-schema/apache-derby-connection-config-schema.json\",\n  \"title\": \"ConnectionConfig\",\n  \"description\": \"JDBC connection configuration for Apache Derby in embedded or client/server mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"Derby deployment mode.\",\n      \"enum\": [\n        \"embedded\",\n        \"client\"\n      ],\n      \"example\": \"embedded\"\n    },\n    \"databaseName\": {\n      \"type\": \"string\",\n      \"description\": \"Database name or path to create/connect to.\",\n      \"example\": \"mydb\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Network Server hostname (client mode only).\",\n      \"example\": \"localhost\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Network Server port (client mode only).\",\n      \"default\": 1527,\n      \"example\": 1527\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Database user (when authentication is enabled).\",\n      \"example\": \"app\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Database password (when authentication is enabled).\",\n      \"example\": \"secretpassword\"\n    },\n    \"createDatabase\": {\n      \"type\": \"string\",\n      \"description\": \"Create the database if it does not exist.\",\n      \"enum\": [\n        \"create\"\n      ],\n      \"example\": \"create\"\n    },\n    \"bootPassword\": {\n      \"type\": \"string\",\n      \"description\": \"Boot password for encrypted databases.\"\n    },\n    \"dataEncryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable data-at-rest encryption for this database.\",\n      \"default\": false,\n      \"example\": false\n\
  \    },\n    \"encryptionAlgorithm\": {\n      \"type\": \"string\",\n      \"description\": \"Encryption algorithm for encrypted databases.\",\n      \"example\": \"AES/CBC/NoPadding\"\n    }\n  },\n  \"required\": [\n    \"mode\",\n    \"databaseName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-derby/refs/heads/main/json-schema/apache-derby-connection-config-schema.json
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
