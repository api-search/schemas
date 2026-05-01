---
description: AggregationResponseList schema
layout: schema
name: AggregationResponseList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-aggregation-response-list-schema.json
slug: inspector-aggregation-response-list
source_filename: inspector-aggregation-response-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aggregation-response-list-schema.json\",\n  \"title\": \"AggregationResponseList\",\n  \"description\": \"AggregationResponseList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"accountAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based on Amazon Web Services account IDs.\"\n          }\n        ]\n      },\n      \"amiAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AmiAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about\
  \ an aggregation response based on Amazon Machine Images (AMIs).\"\n          }\n        ]\n      },\n      \"awsEcrContainerAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsEcrContainerAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based on Amazon ECR container images.\"\n          }\n        ]\n      },\n      \"ec2InstanceAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Ec2InstanceAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based on Amazon EC2 instances.\"\n          }\n        ]\n      },\n      \"findingTypeAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FindingTypeAggregationResponse\"\n          },\n          {\n            \"description\"\
  : \"An object that contains details about an aggregation response based on finding types.\"\n          }\n        ]\n      },\n      \"imageLayerAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ImageLayerAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based on container image layers.\"\n          }\n        ]\n      },\n      \"lambdaFunctionAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LambdaFunctionAggregationResponse\"\n          },\n          {\n            \"description\": \"An aggregation of findings by AWS Lambda function.\"\n          }\n        ]\n      },\n      \"lambdaLayerAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LambdaLayerAggregationResponse\"\n          },\n          {\n            \"description\": \"An aggregation of findings\
  \ by AWS Lambda layer.\"\n          }\n        ]\n      },\n      \"packageAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PackageAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based on operating system package type.\"\n          }\n        ]\n      },\n      \"repositoryAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RepositoryAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based on Amazon ECR repositories.\"\n          }\n        ]\n      },\n      \"titleAggregation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TitleAggregationResponse\"\n          },\n          {\n            \"description\": \"An object that contains details about an aggregation response based\
  \ on finding title.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A structure that contains details about the results of an aggregation type.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aggregation-response-list-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AggregationResponseList
---
