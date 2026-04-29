---
description: Information about a finding that was detected in your code.
layout: schema
name: Finding
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: detectorId
  type: object
- description: ''
  name: detectorName
  type: object
- description: ''
  name: detectorTags
  type: object
- description: ''
  name: generatorId
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: remediation
  type: object
- description: ''
  name: resource
  type: object
- description: ''
  name: ruleId
  type: object
- description: ''
  name: severity
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: title
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: vulnerability
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-finding-schema.json
slug: amazon-codeguru-security-finding
source_filename: amazon-codeguru-security-finding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-schema.json\",\n  \"title\": \"Finding\",\n  \"description\": \"Information about a finding that was detected in your code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the finding was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A description of the finding.\"\n        }\n      ]\n    },\n    \"detectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \"The identifier for the detector that detected the finding in your code. A detector is a defined rule based on industry standards and AWS best practices. \"\n        }\n      ]\n    },\n    \"detectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the detector that identified the security vulnerability in your code. \"\n        }\n      ]\n    },\n    \"detectorTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorTags\"\n        },\n        {\n          \"description\": \"One or more tags or categorizations that are associated with a detector. These tags are defined by type, programming language, or other classification such as maintainability or consistency.\"\n        }\n      ]\n    },\n    \"generatorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \"The identifier for the component that generated a finding such as AWSCodeGuruSecurity or AWSInspector.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier for a finding.\"\n        }\n      ]\n    },\n    \"remediation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Remediation\"\n        },\n        {\n          \"description\": \"An object that contains the details about how to remediate a finding.\"\n        }\n      ]\n    },\n    \"resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Resource\"\n        },\n        {\n          \"description\": \"The resource where Amazon CodeGuru Security detected a finding.\"\n        }\n      ]\n    },\n    \"ruleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n   \
  \       \"description\": \"The identifier for the rule that generated the finding.\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Severity\"\n        },\n        {\n          \"description\": \"The severity of the finding.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of the finding. A finding status can be open or closed. \"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The title of the finding.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of finding. \"\n        }\n      ]\n   \
  \ },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the finding was last updated. Findings are updated when you remediate them or when the finding code location changes. \"\n        }\n      ]\n    },\n    \"vulnerability\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vulnerability\"\n        },\n        {\n          \"description\": \"An object that describes the detected security vulnerability.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: Finding
---
