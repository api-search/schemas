---
description: Request to execute a code statement
layout: schema
name: StatementRequest
properties_list:
- description: Code to execute
  name: code
  type: string
- description: Code type (defaults to session kind)
  name: kind
  type: string
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-statement-request-schema.json
slug: rest-api-statement-request
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: StatementRequest
---
