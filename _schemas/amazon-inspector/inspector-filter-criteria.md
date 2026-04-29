---
description: Details on the criteria used to define the filter.
layout: schema
name: FilterCriteria
properties_list:
- description: ''
  name: awsAccountId
  type: object
- description: ''
  name: codeVulnerabilityDetectorName
  type: object
- description: ''
  name: codeVulnerabilityDetectorTags
  type: object
- description: ''
  name: codeVulnerabilityFilePath
  type: object
- description: ''
  name: componentId
  type: object
- description: ''
  name: componentType
  type: object
- description: ''
  name: ec2InstanceImageId
  type: object
- description: ''
  name: ec2InstanceSubnetId
  type: object
- description: ''
  name: ec2InstanceVpcId
  type: object
- description: ''
  name: ecrImageArchitecture
  type: object
- description: ''
  name: ecrImageHash
  type: object
- description: ''
  name: ecrImagePushedAt
  type: object
- description: ''
  name: ecrImageRegistry
  type: object
- description: ''
  name: ecrImageRepositoryName
  type: object
- description: ''
  name: ecrImageTags
  type: object
- description: ''
  name: epssScore
  type: object
- description: ''
  name: exploitAvailable
  type: object
- description: ''
  name: findingArn
  type: object
- description: ''
  name: findingStatus
  type: object
- description: ''
  name: findingType
  type: object
- description: ''
  name: firstObservedAt
  type: object
- description: ''
  name: fixAvailable
  type: object
- description: ''
  name: inspectorScore
  type: object
- description: ''
  name: lambdaFunctionExecutionRoleArn
  type: object
- description: ''
  name: lambdaFunctionLastModifiedAt
  type: object
- description: ''
  name: lambdaFunctionLayers
  type: object
- description: ''
  name: lambdaFunctionName
  type: object
- description: ''
  name: lambdaFunctionRuntime
  type: object
- description: ''
  name: lastObservedAt
  type: object
- description: ''
  name: networkProtocol
  type: object
- description: ''
  name: portRange
  type: object
- description: ''
  name: relatedVulnerabilities
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: resourceTags
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: severity
  type: object
- description: ''
  name: title
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: vendorSeverity
  type: object
- description: ''
  name: vulnerabilityId
  type: object
- description: ''
  name: vulnerabilitySource
  type: object
- description: ''
  name: vulnerablePackages
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-filter-criteria-schema.json
slug: inspector-filter-criteria
source_filename: inspector-filter-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-filter-criteria-schema.json\",\n  \"title\": \"FilterCriteria\",\n  \"description\": \"Details on the criteria used to define the filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the Amazon Web Services account IDs used to filter findings.\"\n        }\n      ]\n    },\n    \"codeVulnerabilityDetectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The name of the detector used to identify a code vulnerability in a Lambda function used to filter findings.\"\n        }\n      ]\n    },\n    \"codeVulnerabilityDetectorTags\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The detector type tag associated with the vulnerability used to filter findings. Detector tags group related vulnerabilities by common themes or tactics. For a list of available tags by programming language, see <a href=\\\"https://docs.aws.amazon.com/codeguru/detector-library/java/tags/\\\">Java tags</a>, or <a href=\\\"https://docs.aws.amazon.com/codeguru/detector-library/python/tags/\\\">Python tags</a>. \"\n        }\n      ]\n    },\n    \"codeVulnerabilityFilePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The file path to the file in a Lambda function that contains a code vulnerability used to filter findings.\"\n        }\n      ]\n    },\n    \"componentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\
  \n        },\n        {\n          \"description\": \"Details of the component IDs used to filter findings.\"\n        }\n      ]\n    },\n    \"componentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the component types used to filter findings.\"\n        }\n      ]\n    },\n    \"ec2InstanceImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the Amazon EC2 instance image IDs used to filter findings.\"\n        }\n      ]\n    },\n    \"ec2InstanceSubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the Amazon EC2 instance subnet IDs used to filter findings.\"\n        }\n      ]\n    },\n    \"ec2InstanceVpcId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the Amazon EC2 instance VPC IDs used to filter findings.\"\n        }\n      ]\n    },\n    \"ecrImageArchitecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the Amazon ECR image architecture types used to filter findings.\"\n        }\n      ]\n    },\n    \"ecrImageHash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details of the Amazon ECR image hashes used to filter findings.\"\n        }\n      ]\n    },\n    \"ecrImagePushedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateFilterList\"\n        },\n        {\n          \"description\": \"Details on the Amazon ECR image push date and\
  \ time used to filter findings.\"\n        }\n      ]\n    },\n    \"ecrImageRegistry\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the Amazon ECR registry used to filter findings.\"\n        }\n      ]\n    },\n    \"ecrImageRepositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the name of the Amazon ECR repository used to filter findings.\"\n        }\n      ]\n    },\n    \"ecrImageTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The tags attached to the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"epssScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberFilterList\"\n        },\n \
  \       {\n          \"description\": \"The EPSS score used to filter findings.\"\n        }\n      ]\n    },\n    \"exploitAvailable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Filters the list of AWS Lambda findings by the availability of exploits.\"\n        }\n      ]\n    },\n    \"findingArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the finding ARNs used to filter findings.\"\n        }\n      ]\n    },\n    \"findingStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the finding status types used to filter findings.\"\n        }\n      ]\n    },\n    \"findingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\
  \n        },\n        {\n          \"description\": \"Details on the finding types used to filter findings.\"\n        }\n      ]\n    },\n    \"firstObservedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateFilterList\"\n        },\n        {\n          \"description\": \"Details on the date and time a finding was first seen used to filter findings.\"\n        }\n      ]\n    },\n    \"fixAvailable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on whether a fix is available through a version update. This value can be <code>YES</code>, <code>NO</code>, or <code>PARTIAL</code>. A <code>PARTIAL</code> fix means that some, but not all, of the packages identified in the finding have fixes available through updated versions.\"\n        }\n      ]\n    },\n    \"inspectorScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberFilterList\"\
  \n        },\n        {\n          \"description\": \"The Amazon Inspector score to filter on.\"\n        }\n      ]\n    },\n    \"lambdaFunctionExecutionRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Filters the list of AWS Lambda functions by execution role.\"\n        }\n      ]\n    },\n    \"lambdaFunctionLastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateFilterList\"\n        },\n        {\n          \"description\": \"Filters the list of AWS Lambda functions by the date and time that a user last updated the configuration, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601 format</a> \"\n        }\n      ]\n    },\n    \"lambdaFunctionLayers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\":\
  \ \"Filters the list of AWS Lambda functions by the function's <a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html\\\"> layers</a>. A Lambda function can have up to five layers.\"\n        }\n      ]\n    },\n    \"lambdaFunctionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Filters the list of AWS Lambda functions by the name of the function.\"\n        }\n      ]\n    },\n    \"lambdaFunctionRuntime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Filters the list of AWS Lambda functions by the runtime environment for the Lambda function.\"\n        }\n      ]\n    },\n    \"lastObservedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateFilterList\"\n        },\n        {\n          \"description\": \"Details\
  \ on the date and time a finding was last seen used to filter findings.\"\n        }\n      ]\n    },\n    \"networkProtocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on network protocol used to filter findings.\"\n        }\n      ]\n    },\n    \"portRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRangeFilterList\"\n        },\n        {\n          \"description\": \"Details on the port ranges used to filter findings.\"\n        }\n      ]\n    },\n    \"relatedVulnerabilities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the related vulnerabilities used to filter findings.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\
  \n        },\n        {\n          \"description\": \"Details on the resource IDs used to filter findings.\"\n        }\n      ]\n    },\n    \"resourceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapFilterList\"\n        },\n        {\n          \"description\": \"Details on the resource tags used to filter findings.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the resource types used to filter findings.\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the severity used to filter findings.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\
  \n        },\n        {\n          \"description\": \"Details on the finding title used to filter findings.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateFilterList\"\n        },\n        {\n          \"description\": \"Details on the date and time a finding was last updated at used to filter findings.\"\n        }\n      ]\n    },\n    \"vendorSeverity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the vendor severity used to filter findings.\"\n        }\n      ]\n    },\n    \"vulnerabilityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the vulnerability ID used to filter findings.\"\n        }\n      ]\n    },\n    \"vulnerabilitySource\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"Details on the vulnerability type used to filter findings.\"\n        }\n      ]\n    },\n    \"vulnerablePackages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFilterList\"\n        },\n        {\n          \"description\": \"Details on the vulnerable packages used to filter findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-filter-criteria-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FilterCriteria
---
