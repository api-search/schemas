---
description: A structure that contains details about the results of an aggregation type.
layout: schema
name: AggregationResponse
properties_list:
- description: ''
  name: accountAggregation
  type: object
- description: ''
  name: amiAggregation
  type: object
- description: ''
  name: awsEcrContainerAggregation
  type: object
- description: ''
  name: ec2InstanceAggregation
  type: object
- description: ''
  name: findingTypeAggregation
  type: object
- description: ''
  name: imageLayerAggregation
  type: object
- description: ''
  name: lambdaFunctionAggregation
  type: object
- description: ''
  name: lambdaLayerAggregation
  type: object
- description: ''
  name: packageAggregation
  type: object
- description: ''
  name: repositoryAggregation
  type: object
- description: ''
  name: titleAggregation
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-aggregation-response-schema.json
slug: inspector-aggregation-response
source_filename: inspector-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aggregation-response-schema.json\",\n  \"title\": \"AggregationResponse\",\n  \"description\": \"A structure that contains details about the results of an aggregation type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on Amazon Web Services account IDs.\"\n        }\n      ]\n    },\n    \"amiAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on Amazon\
  \ Machine Images (AMIs).\"\n        }\n      ]\n    },\n    \"awsEcrContainerAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsEcrContainerAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on Amazon ECR container images.\"\n        }\n      ]\n    },\n    \"ec2InstanceAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2InstanceAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on Amazon EC2 instances.\"\n        }\n      ]\n    },\n    \"findingTypeAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingTypeAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on finding types.\"\n      \
  \  }\n      ]\n    },\n    \"imageLayerAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageLayerAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on container image layers.\"\n        }\n      ]\n    },\n    \"lambdaFunctionAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionAggregationResponse\"\n        },\n        {\n          \"description\": \"An aggregation of findings by AWS Lambda function.\"\n        }\n      ]\n    },\n    \"lambdaLayerAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaLayerAggregationResponse\"\n        },\n        {\n          \"description\": \"An aggregation of findings by AWS Lambda layer.\"\n        }\n      ]\n    },\n    \"packageAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageAggregationResponse\"\
  \n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on operating system package type.\"\n        }\n      ]\n    },\n    \"repositoryAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on Amazon ECR repositories.\"\n        }\n      ]\n    },\n    \"titleAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TitleAggregationResponse\"\n        },\n        {\n          \"description\": \"An object that contains details about an aggregation response based on finding title.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AggregationResponse
---
