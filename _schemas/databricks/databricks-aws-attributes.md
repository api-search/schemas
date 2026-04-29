---
description: ''
layout: schema
name: AwsAttributes
properties_list:
- description: Number of on-demand instances to place first.
  name: first_on_demand
  type: integer
- description: ''
  name: availability
  type: string
- description: The availability zone identifier (e.g., us-west-2a).
  name: zone_id
  type: string
- description: IAM instance profile ARN for the cluster instances.
  name: instance_profile_arn
  type: string
- description: Max bid price as percentage of on-demand price.
  name: spot_bid_price_percent
  type: integer
- description: ''
  name: ebs_volume_type
  type: string
- description: ''
  name: ebs_volume_count
  type: integer
- description: ''
  name: ebs_volume_size
  type: integer
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-aws-attributes-schema.json
slug: databricks-aws-attributes
source_filename: databricks-aws-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AwsAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_on_demand\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of on-demand instances to place first.\"\n    },\n    \"availability\": {\n      \"type\": \"string\"\n    },\n    \"zone_id\": {\n      \"type\": \"string\",\n      \"description\": \"The availability zone identifier (e.g., us-west-2a).\"\n    },\n    \"instance_profile_arn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM instance profile ARN for the cluster instances.\"\n    },\n    \"spot_bid_price_percent\": {\n      \"type\": \"integer\",\n      \"description\": \"Max bid price as percentage of on-demand price.\"\n    },\n    \"ebs_volume_type\": {\n      \"type\": \"string\"\n    },\n    \"ebs_volume_count\": {\n      \"type\": \"integer\"\n    },\n    \"ebs_volume_size\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-aws-attributes-schema.json
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
title: AwsAttributes
---
