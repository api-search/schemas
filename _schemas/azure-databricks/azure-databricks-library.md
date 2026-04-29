---
description: ''
layout: schema
name: Library
properties_list:
- description: URI of the JAR library to install
  name: jar
  type: string
- description: URI of the egg library to install
  name: egg
  type: string
- description: URI of the wheel library to install
  name: whl
  type: string
- description: ''
  name: pypi
  type: object
- description: ''
  name: maven
  type: object
- description: ''
  name: cran
  type: object
- description: Path to a requirements.txt file. Only supported on clusters running Databricks Runtime 15.0+.
  name: requirements
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-library-schema.json
slug: azure-databricks-library
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Library\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jar\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the JAR library to install\"\n    },\n    \"egg\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the egg library to install\"\n    },\n    \"whl\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the wheel library to install\"\n    },\n    \"pypi\": {\n      \"type\": \"object\"\n    },\n    \"maven\": {\n      \"type\": \"object\"\n    },\n    \"cran\": {\n      \"type\": \"object\"\n    },\n    \"requirements\": {\n      \"type\": \"string\",\n      \"description\": \"Path to a requirements.txt file. Only supported on clusters running Databricks Runtime 15.0+.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-library-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: Library
---
