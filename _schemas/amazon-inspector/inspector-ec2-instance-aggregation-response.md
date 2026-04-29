---
description: A response that contains the results of a finding aggregation by Amazon EC2 instance.
layout: schema
name: Ec2InstanceAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: ami
  type: object
- description: ''
  name: instanceId
  type: object
- description: ''
  name: instanceTags
  type: object
- description: ''
  name: networkFindings
  type: object
- description: ''
  name: operatingSystem
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-ec2-instance-aggregation-response-schema.json
slug: inspector-ec2-instance-aggregation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ec2-instance-aggregation-response-schema.json\",\n  \"title\": \"Ec2InstanceAggregationResponse\",\n  \"description\": \"A response that contains the results of a finding aggregation by Amazon EC2 instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account for the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"ami\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiId\"\n        },\n        {\n          \"description\": \"The Amazon Machine Image (AMI) of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"instanceId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instance ID.\"\n        }\n      ]\n    },\n    \"instanceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags attached to the instance.\"\n        }\n      ]\n    },\n    \"networkFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of network findings for the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"operatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The operating system of the Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\
  \n        },\n        {\n          \"description\": \"An object that contains the count of matched findings per severity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ec2-instance-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Ec2InstanceAggregationResponse
---
