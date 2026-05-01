---
description: The estimated monthly savings after you adjust the configurations of your instances running on the inferred workload types to the recommended configurations. If the <code>inferredWorkloadTypes</code> list contains multiple entries, then the savings are the sum of the monthly savings from instances that run the exact combination of the inferred workload types.
layout: schema
name: InferredWorkloadSaving
properties_list:
- description: ''
  name: inferredWorkloadTypes
  type: object
- description: ''
  name: estimatedMonthlySavings
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-inferred-workload-saving-schema.json
slug: compute-optimizer-inferred-workload-saving
source_filename: compute-optimizer-inferred-workload-saving-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-inferred-workload-saving-schema.json\",\n  \"title\": \"InferredWorkloadSaving\",\n  \"description\": \" The estimated monthly savings after you adjust the configurations of your instances running on the inferred workload types to the recommended configurations. If the <code>inferredWorkloadTypes</code> list contains multiple entries, then the savings are the sum of the monthly savings from instances that run the exact combination of the inferred workload types. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inferredWorkloadTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferredWorkloadTypes\"\n        },\n        {\n          \"description\": \"<p>The applications that might be running on the instance as inferred by Compute Optimizer.</p>\
  \ <p>Compute Optimizer can infer if one of the following applications might be running on the instance:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instance.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instance.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instance.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instance.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instance.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instance.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instance.</p> </li> <li> <p> <code>Kafka</code> - Infers that Kafka might be running on the instance.</p> </li> <li> <p> <code>SQLServer</code> - Infers that SQLServer might be running on the instance.</p>\
  \ </li> </ul>\"\n        }\n      ]\n    },\n    \"estimatedMonthlySavings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EstimatedMonthlySavings\"\n        },\n        {\n          \"description\": \"An object that describes the estimated monthly savings amount possible by adopting Compute Optimizer recommendations for a given resource. This is based on the On-Demand instance pricing.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-inferred-workload-saving-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: InferredWorkloadSaving
---
