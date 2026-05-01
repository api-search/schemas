---
description: Response from the DescribeTargetGroups action
layout: schema
name: DescribeTargetGroupsResponse
properties_list:
- description: Information about the target groups
  name: targetGroups
  type: array
- description: The marker to use for the next set of results
  name: nextMarker
  type: string
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-describe-target-groups-response-schema.json
slug: amazon-elastic-load-balancing-describe-target-groups-response
source_filename: amazon-elastic-load-balancing-describe-target-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-describe-target-groups-response-schema.json\",\n  \"title\": \"DescribeTargetGroupsResponse\",\n  \"description\": \"Response from the DescribeTargetGroups action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the target groups\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TargetGroup\"\n      }\n    },\n    \"nextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"The marker to use for the next set of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-describe-target-groups-response-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: DescribeTargetGroupsResponse
---
