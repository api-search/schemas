---
description: Schema defining the structure of an Amazon Inspector vulnerability finding, including severity, resource details, vulnerability information, and remediation guidance.
layout: schema
name: Amazon Inspector Finding Definition
properties_list:
- description: The Amazon Resource Name (ARN) of the finding.
  name: findingArn
  type: string
- description: The severity of the finding.
  name: severity
  type: string
- description: The status of the finding.
  name: status
  type: string
- description: The type of the finding.
  name: type
  type: string
- description: The title of the finding.
  name: title
  type: string
- description: The description of the finding.
  name: description
  type: string
- description: The AWS account ID associated with the finding.
  name: awsAccountId
  type: string
- description: The date and time the finding was first observed.
  name: firstObservedAt
  type: string
- description: The date and time the finding was last observed.
  name: lastObservedAt
  type: string
- description: The date and time the finding was last updated.
  name: updatedAt
  type: string
- description: The Amazon Inspector score for the finding.
  name: inspectorScore
  type: number
- description: The resources affected by the finding.
  name: resources
  type: array
- description: ''
  name: remediation
  type: object
- description: ''
  name: packageVulnerabilityDetails
  type: object
- description: ''
  name: networkReachabilityDetails
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/amazon-inspector-schema.json
slug: amazon-inspector
source_filename: amazon-inspector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-inspector/finding-definition\",\n  \"title\": \"Amazon Inspector Finding Definition\",\n  \"description\": \"Schema defining the structure of an Amazon Inspector vulnerability finding, including severity, resource details, vulnerability information, and remediation guidance.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"findingArn\",\n    \"severity\",\n    \"status\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"findingArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the finding.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INFORMATIONAL\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\",\n        \"UNTRIAGED\"\n      ],\n      \"description\": \"The severity of the finding.\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"SUPPRESSED\",\n        \"CLOSED\"\n      ],\n      \"description\": \"The status of the finding.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NETWORK_REACHABILITY\",\n        \"PACKAGE_VULNERABILITY\",\n        \"CODE_VULNERABILITY\"\n      ],\n      \"description\": \"The type of the finding.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the finding.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the finding.\"\n    },\n    \"awsAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID associated with the finding.\"\n    },\n    \"firstObservedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the finding was first observed.\"\n    },\n    \"lastObservedAt\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the finding was last observed.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the finding was last updated.\"\n    },\n    \"inspectorScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n      \"description\": \"The Amazon Inspector score for the finding.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Resource\"\n      },\n      \"description\": \"The resources affected by the finding.\"\n    },\n    \"remediation\": {\n      \"$ref\": \"#/$defs/Remediation\"\n    },\n    \"packageVulnerabilityDetails\": {\n      \"$ref\": \"#/$defs/PackageVulnerabilityDetails\"\n    },\n    \"networkReachabilityDetails\": {\n      \"$ref\": \"#/$defs/NetworkReachabilityDetails\"\n    }\n  },\n  \"$defs\": {\n    \"Resource\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"A resource affected by a finding.\",\n      \"required\": [\n        \"id\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the resource.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"AWS_EC2_INSTANCE\",\n            \"AWS_ECR_CONTAINER_IMAGE\",\n            \"AWS_ECR_REPOSITORY\",\n            \"AWS_LAMBDA_FUNCTION\"\n          ],\n          \"description\": \"The type of the resource.\"\n        },\n        \"partition\": {\n          \"type\": \"string\",\n          \"description\": \"The partition of the resource.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"The AWS region of the resource.\"\n        },\n        \"tags\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\"\
  : \"string\"\n          },\n          \"description\": \"Tags associated with the resource.\"\n        }\n      }\n    },\n    \"Remediation\": {\n      \"type\": \"object\",\n      \"description\": \"Remediation guidance for a finding.\",\n      \"properties\": {\n        \"recommendation\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"text\": {\n              \"type\": \"string\",\n              \"description\": \"The recommended remediation action.\"\n            },\n            \"Url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"A URL for more information about the remediation.\"\n            }\n          }\n        }\n      }\n    },\n    \"PackageVulnerabilityDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details about a package vulnerability finding.\",\n      \"properties\": {\n        \"vulnerabilityId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The ID of the vulnerability (e.g., CVE ID).\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The source of the vulnerability information.\"\n        },\n        \"sourceUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URL to the source of the vulnerability information.\"\n        },\n        \"cvss\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"version\": {\n                \"type\": \"string\"\n              },\n              \"baseScore\": {\n                \"type\": \"number\"\n              },\n              \"scoringVector\": {\n                \"type\": \"string\"\n              },\n              \"source\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"description\": \"CVSS scores for the vulnerability.\"\n        },\n \
  \       \"vulnerablePackages\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"version\": {\n                \"type\": \"string\"\n              },\n              \"fixedInVersion\": {\n                \"type\": \"string\"\n              },\n              \"packageManager\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"description\": \"The packages affected by the vulnerability.\"\n        }\n      }\n    },\n    \"NetworkReachabilityDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details about a network reachability finding.\",\n      \"properties\": {\n        \"protocol\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"TCP\",\n            \"UDP\"\n          ],\n          \"description\": \"The protocol associated\
  \ with the finding.\"\n        },\n        \"openPortRange\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"begin\": {\n              \"type\": \"integer\"\n            },\n            \"end\": {\n              \"type\": \"integer\"\n            }\n          },\n          \"description\": \"The open port range.\"\n        },\n        \"networkPath\": {\n          \"type\": \"object\",\n          \"description\": \"The network path details.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/amazon-inspector-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Amazon Inspector Finding Definition
---
