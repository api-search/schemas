---
description: A structure that identifies filter criteria for <code>GetCoverageStatistics</code>.
layout: schema
name: CoverageFilterCriteria
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: ec2InstanceTags
  type: object
- description: ''
  name: ecrImageTags
  type: object
- description: ''
  name: ecrRepositoryName
  type: object
- description: ''
  name: lambdaFunctionName
  type: object
- description: ''
  name: lambdaFunctionRuntime
  type: object
- description: ''
  name: lambdaFunctionTags
  type: object
- description: ''
  name: lastScannedAt
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: scanStatusCode
  type: object
- description: ''
  name: scanStatusReason
  type: object
- description: ''
  name: scanType
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-coverage-filter-criteria-schema.json
slug: inspector-coverage-filter-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-coverage-filter-criteria-schema.json\",\n  \"title\": \"CoverageFilterCriteria\",\n  \"description\": \"A structure that identifies filter criteria for <code>GetCoverageStatistics</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"An array of Amazon Web Services account IDs to return coverage statistics for.\"\n        }\n      ]\n    },\n    \"ec2InstanceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageMapFilterList\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instance tags to filter on.\"\n        }\n      ]\n    },\n    \"ecrImageTags\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"The Amazon ECR image tags to filter on.\"\n        }\n      ]\n    },\n    \"ecrRepositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"The Amazon ECR repository name to filter on.\"\n        }\n      ]\n    },\n    \"lambdaFunctionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"Returns coverage statistics for AWS Lambda functions filtered by function names.\"\n        }\n      ]\n    },\n    \"lambdaFunctionRuntime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"Returns coverage statistics for\
  \ AWS Lambda functions filtered by runtime.\"\n        }\n      ]\n    },\n    \"lambdaFunctionTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageMapFilterList\"\n        },\n        {\n          \"description\": \"Returns coverage statistics for AWS Lambda functions filtered by tag.\"\n        }\n      ]\n    },\n    \"lastScannedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageDateFilterList\"\n        },\n        {\n          \"description\": \"Filters Amazon Web Services resources based on whether Amazon Inspector has checked them for vulnerabilities within the specified time range.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"An array of Amazon Web Services resource IDs to return coverage statistics for.\"\n        }\n      ]\n    },\n  \
  \  \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"An array of Amazon Web Services resource types to return coverage statistics for. The values can be <code>AWS_EC2_INSTANCE</code>, <code>AWS_LAMBDA_FUNCTION</code> or <code>AWS_ECR_REPOSITORY</code>.\"\n        }\n      ]\n    },\n    \"scanStatusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"The scan status code to filter on.\"\n        }\n      ]\n    },\n    \"scanStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\n        },\n        {\n          \"description\": \"The scan status reason to filter on.\"\n        }\n      ]\n    },\n    \"scanType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStringFilterList\"\
  \n        },\n        {\n          \"description\": \"An array of Amazon Inspector scan types to return coverage statistics for.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-coverage-filter-criteria-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CoverageFilterCriteria
---
