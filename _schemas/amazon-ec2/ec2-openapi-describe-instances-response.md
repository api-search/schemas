---
description: Response from the DescribeInstances action
layout: schema
name: DescribeInstancesResponse
properties_list:
- description: Information about the reservations
  name: reservationSet
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon EC2
provider_slug: amazon-ec2
schema_file: json-schema/ec2-openapi-describe-instances-response-schema.json
slug: ec2-openapi-describe-instances-response
source_filename: ec2-openapi-describe-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-describe-instances-response-schema.json\",\n  \"title\": \"DescribeInstancesResponse\",\n  \"description\": \"Response from the DescribeInstances action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reservationSet\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the reservations\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"reservationId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the reservation\"\n          },\n          \"instancesSet\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Instance\"\n            }\n          }\n        }\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-describe-instances-response-schema.json
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
title: DescribeInstancesResponse
---
