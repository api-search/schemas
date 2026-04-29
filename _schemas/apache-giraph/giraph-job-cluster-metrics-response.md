---
description: YARN cluster metrics response
layout: schema
name: ClusterMetricsResponse
properties_list:
- description: Cluster resource metrics
  name: clusterMetrics
  type: object
provider_name: Apache Giraph
provider_slug: apache-giraph
schema_file: json-schema/giraph-job-cluster-metrics-response-schema.json
slug: giraph-job-cluster-metrics-response
source_filename: giraph-job-cluster-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-cluster-metrics-response-schema.json\",\n  \"title\": \"ClusterMetricsResponse\",\n  \"description\": \"YARN cluster metrics response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterMetrics\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster resource metrics\",\n      \"properties\": {\n        \"activeNodes\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of active nodes\",\n          \"example\": \"5\"\n        },\n        \"totalMB\": {\n          \"type\": \"integer\",\n          \"description\": \"Total cluster memory in MB\",\n          \"example\": \"40960\"\n        },\n        \"availableMB\": {\n          \"type\": \"integer\",\n          \"description\": \"Available memory in MB\",\n          \"example\": \"20480\"\n        },\n\
  \        \"totalVirtualCores\": {\n          \"type\": \"integer\",\n          \"description\": \"Total virtual CPU cores\",\n          \"example\": \"20\"\n        },\n        \"availableVirtualCores\": {\n          \"type\": \"integer\",\n          \"description\": \"Available virtual CPU cores\",\n          \"example\": \"10\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-cluster-metrics-response-schema.json
tags:
- Apache
- Big Data
- BSP
- Graph Processing
- Hadoop
- Open Source
- Retired
title: ClusterMetricsResponse
---
