---
description: ''
layout: schema
name: Library
properties_list:
- description: URI of a JAR to install.
  name: jar
  type: string
- description: URI of an egg to install (deprecated).
  name: egg
  type: string
- description: URI of a wheel to install.
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
- description: Path to a requirements.txt file.
  name: requirements
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-library-schema.json
slug: databricks-library
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Library\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jar\": {\n      \"type\": \"string\",\n      \"description\": \"URI of a JAR to install.\"\n    },\n    \"egg\": {\n      \"type\": \"string\",\n      \"description\": \"URI of an egg to install (deprecated).\"\n    },\n    \"whl\": {\n      \"type\": \"string\",\n      \"description\": \"URI of a wheel to install.\"\n    },\n    \"pypi\": {\n      \"type\": \"object\"\n    },\n    \"maven\": {\n      \"type\": \"object\"\n    },\n    \"cran\": {\n      \"type\": \"object\"\n    },\n    \"requirements\": {\n      \"type\": \"string\",\n      \"description\": \"Path to a requirements.txt file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-library-schema.json
tags:
- AI
- Analytics
- Apache Spark
- Big Data
- Clean Rooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
title: Library
---
