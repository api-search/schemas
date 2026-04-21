---
description: An interactive Spark session
layout: schema
name: Session
properties_list:
- description: Session identifier
  name: id
  type: integer
- description: Spark application ID
  name: appId
  type: string
- description: Session owner
  name: owner
  type: string
- description: Proxy user for the session
  name: proxyUser
  type: string
- description: Session type
  name: kind
  type: string
- description: Recent log lines
  name: log
  type: array
- description: Session state
  name: state
  type: string
- description: Spark application information
  name: appInfo
  type: object
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-session-schema.json
slug: rest-api-session
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Session
---
