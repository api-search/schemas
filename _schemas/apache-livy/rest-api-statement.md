---
description: A code statement executed in a session
layout: schema
name: Statement
properties_list:
- description: Statement identifier
  name: id
  type: integer
- description: The code that was executed
  name: code
  type: string
- description: Statement execution state
  name: state
  type: string
- description: Statement output
  name: output
  type: object
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-statement-schema.json
slug: rest-api-statement
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Statement
---
