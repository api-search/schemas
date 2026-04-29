---
description: DescribeMetricCollectionTypesAnswer schema from Auto Scaling
layout: schema
name: DescribeMetricCollectionTypesAnswer
properties_list:
- description: ''
  name: Metrics
  type: object
- description: ''
  name: Granularities
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-metric-collection-types-answer-schema.json
slug: ec2-auto-scaling-describe-metric-collection-types-answer
source_filename: ec2-auto-scaling-describe-metric-collection-types-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-metric-collection-types-answer-schema.json\",\n  \"title\": \"DescribeMetricCollectionTypesAnswer\",\n  \"description\": \"DescribeMetricCollectionTypesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricCollectionTypes\"\n        },\n        {\n          \"description\": \"The metrics.\"\n        }\n      ]\n    },\n    \"Granularities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricGranularityTypes\"\n        },\n        {\n          \"description\": \"The granularities for the metrics.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Granularities\": [\n      {\n        \"Granularity\": \"\
  1Minute\"\n      }\n    ],\n    \"Metrics\": [\n      {\n        \"Metric\": \"GroupMinSize\"\n      },\n      {\n        \"Metric\": \"GroupMaxSize\"\n      },\n      {\n        \"Metric\": \"GroupDesiredCapacity\"\n      },\n      {\n        \"Metric\": \"GroupInServiceInstances\"\n      },\n      {\n        \"Metric\": \"GroupPendingInstances\"\n      },\n      {\n        \"Metric\": \"GroupTerminatingInstances\"\n      },\n      {\n        \"Metric\": \"GroupStandbyInstances\"\n      },\n      {\n        \"Metric\": \"GroupTotalInstances\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-metric-collection-types-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeMetricCollectionTypesAnswer
---
