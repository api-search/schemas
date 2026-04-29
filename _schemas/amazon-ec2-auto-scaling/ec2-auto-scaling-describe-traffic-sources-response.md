---
description: DescribeTrafficSourcesResponse schema from Auto Scaling
layout: schema
name: DescribeTrafficSourcesResponse
properties_list:
- description: ''
  name: TrafficSources
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-traffic-sources-response-schema.json
slug: ec2-auto-scaling-describe-traffic-sources-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-traffic-sources-response-schema.json\",\n  \"title\": \"DescribeTrafficSourcesResponse\",\n  \"description\": \"DescribeTrafficSourcesResponse schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TrafficSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficSourceStates\"\n        },\n        {\n          \"description\": \"Information about the traffic sources.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"This string indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for\
  \ the <code>NextToken</code> value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"NextToken\": \"\",\n    \"TrafficSources\": [\n      {\n        \"Identifier\": \"arn:aws:vpc-lattice:us-west-2:123456789012:targetgroup/tg-0e2f2665eEXAMPLE\",\n        \"State\": \"InService\",\n        \"Type\": \"vpc-lattice\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-traffic-sources-response-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeTrafficSourcesResponse
---
