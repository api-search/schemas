---
description: Contains details about a vulnerability scan finding.
layout: schema
name: ImageScanFinding
properties_list:
- description: ''
  name: awsAccountId
  type: object
- description: ''
  name: imageBuildVersionArn
  type: object
- description: ''
  name: imagePipelineArn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: title
  type: object
- description: ''
  name: remediation
  type: object
- description: ''
  name: severity
  type: object
- description: ''
  name: firstObservedAt
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: inspectorScore
  type: object
- description: ''
  name: inspectorScoreDetails
  type: object
- description: ''
  name: packageVulnerabilityDetails
  type: object
- description: ''
  name: fixAvailable
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-finding-schema.json
slug: ec2-image-builder-image-scan-finding
source_filename: ec2-image-builder-image-scan-finding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-finding-schema.json\",\n  \"title\": \"ImageScanFinding\",\n  \"description\": \"Contains details about a vulnerability scan finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID that's associated with the finding.\"\n        }\n      ]\n    },\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image build version that's associated with the finding.\"\n        }\n      ]\n    },\n    \"imagePipelineArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePipelineArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image pipeline that's associated with the finding.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The type of the finding. Image Builder looks for findings of the type <code>PACKAGE_VULNERABILITY</code> that apply to output images, and excludes other types.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the finding.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"\
  description\": \"The title of the finding.\"\n        }\n      ]\n    },\n    \"remediation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Remediation\"\n        },\n        {\n          \"description\": \"An object that contains the details about how to remediate the finding.\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The severity of the finding.\"\n        }\n      ]\n    },\n    \"firstObservedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeTimestamp\"\n        },\n        {\n          \"description\": \"The date and time when the finding was first observed.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeTimestamp\"\n        },\n        {\n          \"description\": \"The\
  \ timestamp when the finding was last updated.\"\n        }\n      ]\n    },\n    \"inspectorScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeDouble\"\n        },\n        {\n          \"description\": \"The score that Amazon Inspector assigned for the finding.\"\n        }\n      ]\n    },\n    \"inspectorScoreDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InspectorScoreDetails\"\n        },\n        {\n          \"description\": \"An object that contains details of the Amazon Inspector score.\"\n        }\n      ]\n    },\n    \"packageVulnerabilityDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVulnerabilityDetails\"\n        },\n        {\n          \"description\": \"An object that contains the details of a package vulnerability finding.\"\n        }\n      ]\n    },\n    \"fixAvailable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\
  \n        },\n        {\n          \"description\": \"Details about whether a fix is available for any of the packages that are identified in the finding through a version update.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-finding-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanFinding
---
