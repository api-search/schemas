---
description: Information about a vulnerable package that Amazon Inspector identifies in a finding.
layout: schema
name: VulnerablePackage
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: sourceLayerHash
  type: object
- description: ''
  name: epoch
  type: object
- description: ''
  name: release
  type: object
- description: ''
  name: arch
  type: object
- description: ''
  name: packageManager
  type: object
- description: ''
  name: filePath
  type: object
- description: ''
  name: fixedInVersion
  type: object
- description: ''
  name: remediation
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-vulnerable-package-schema.json
slug: ec2-image-builder-vulnerable-package
source_filename: ec2-image-builder-vulnerable-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-vulnerable-package-schema.json\",\n  \"title\": \"VulnerablePackage\",\n  \"description\": \"Information about a vulnerable package that Amazon Inspector identifies in a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the vulnerable package.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The version of the vulnerable package.\"\n        }\n      ]\n    },\n    \"sourceLayerHash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceLayerHash\"\
  \n        },\n        {\n          \"description\": \"The source layer hash of the vulnerable package.\"\n        }\n      ]\n    },\n    \"epoch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageEpoch\"\n        },\n        {\n          \"description\": \"The epoch of the vulnerable package.\"\n        }\n      ]\n    },\n    \"release\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The release of the vulnerable package.\"\n        }\n      ]\n    },\n    \"arch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageArchitecture\"\n        },\n        {\n          \"description\": \"The architecture of the vulnerable package.\"\n        }\n      ]\n    },\n    \"packageManager\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\"\
  : \"The package manager of the vulnerable package.\"\n        }\n      ]\n    },\n    \"filePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The file path of the vulnerable package.\"\n        }\n      ]\n    },\n    \"fixedInVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The version of the package that contains the vulnerability fix.\"\n        }\n      ]\n    },\n    \"remediation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The code to run in your environment to update packages with a fix available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-vulnerable-package-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: VulnerablePackage
---
