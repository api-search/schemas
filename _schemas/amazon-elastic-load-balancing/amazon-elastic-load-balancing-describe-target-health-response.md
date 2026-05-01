---
description: Response from the DescribeTargetHealth action
layout: schema
name: DescribeTargetHealthResponse
properties_list:
- description: Information about the health of the targets
  name: targetHealthDescriptions
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-describe-target-health-response-schema.json
slug: amazon-elastic-load-balancing-describe-target-health-response
source_filename: amazon-elastic-load-balancing-describe-target-health-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-describe-target-health-response-schema.json\",\n  \"title\": \"DescribeTargetHealthResponse\",\n  \"description\": \"Response from the DescribeTargetHealth action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetHealthDescriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the health of the targets\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"target\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the target\"\n              },\n              \"port\": {\n                \"type\": \"integer\",\n                \"description\": \"The port\
  \ on which the target is listening\"\n              }\n            }\n          },\n          \"targetHealth\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"state\": {\n                \"type\": \"string\",\n                \"description\": \"The state of the target\",\n                \"enum\": [\n                  \"initial\",\n                  \"healthy\",\n                  \"unhealthy\",\n                  \"unused\",\n                  \"draining\",\n                  \"unavailable\"\n                ]\n              },\n              \"reason\": {\n                \"type\": \"string\",\n                \"description\": \"The reason code\"\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"A description of the target health\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-describe-target-health-response-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: DescribeTargetHealthResponse
---
