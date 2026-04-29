---
description: A security scan result representing a vulnerability or finding detected by Checkmarx scanning engines (SAST, SCA, KICS) across static code analysis, open source dependency analysis, and infrastructure-as-code scanning.
layout: schema
name: Checkmarx Scan Result
properties_list:
- description: Unique identifier for the scan result
  name: id
  type: string
- description: Stable identifier for tracking the same finding across multiple scans
  name: similarityId
  type: string
- description: Identifier of the scan that produced this result
  name: scanId
  type: string
- description: Identifier of the project being scanned
  name: projectId
  type: string
- description: The scanning engine that detected this finding
  name: type
  type: string
- description: Severity level of the finding
  name: severity
  type: string
- description: Whether the finding is newly detected or recurring from previous scans
  name: status
  type: string
- description: Triage state indicating how the finding has been evaluated
  name: state
  type: string
- description: Human-readable description of the vulnerability or finding
  name: description
  type: string
- description: Name of the SAST query or rule that detected the finding
  name: queryName
  type: string
- description: Category or group the detecting query belongs to
  name: queryGroup
  type: string
- description: Programming language of the scanned source code
  name: languageName
  type: string
- description: ''
  name: vulnerabilityDetails
  type: object
- description: ''
  name: location
  type: object
- description: Ordered list of code flow nodes showing the data flow path from source to sink (SAST findings)
  name: codeFlow
  type: array
- description: ''
  name: packageData
  type: object
- description: Timestamp when this finding was first detected
  name: firstFoundAt
  type: string
- description: Timestamp when this finding was detected in the current scan
  name: foundAt
  type: string
- description: Triage comments added by security reviewers
  name: comments
  type: array
provider_name: Checkmarx
provider_slug: checkmarx
schema_file: json-schema/checkmarx-scan-result-schema.json
slug: checkmarx-scan-result
source_filename: checkmarx-scan-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://checkmarx.com/schemas/checkmarx/scan-result.json\",\n  \"title\": \"Checkmarx Scan Result\",\n  \"description\": \"A security scan result representing a vulnerability or finding detected by Checkmarx scanning engines (SAST, SCA, KICS) across static code analysis, open source dependency analysis, and infrastructure-as-code scanning.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"severity\", \"type\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the scan result\"\n    },\n    \"similarityId\": {\n      \"type\": \"string\",\n      \"description\": \"Stable identifier for tracking the same finding across multiple scans\"\n    },\n    \"scanId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Identifier of the scan that produced this\
  \ result\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Identifier of the project being scanned\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"sast\", \"sca\", \"kics\", \"apisec\"],\n      \"description\": \"The scanning engine that detected this finding\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"CRITICAL\", \"HIGH\", \"MEDIUM\", \"LOW\", \"INFO\"],\n      \"description\": \"Severity level of the finding\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"NEW\", \"RECURRENT\"],\n      \"description\": \"Whether the finding is newly detected or recurring from previous scans\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"TO_VERIFY\", \"NOT_EXPLOITABLE\", \"PROPOSED_NOT_EXPLOITABLE\", \"CONFIRMED\", \"URGENT\"],\n      \"description\": \"Triage state indicating how the finding has been evaluated\"\n\
  \    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the vulnerability or finding\"\n    },\n    \"queryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SAST query or rule that detected the finding\"\n    },\n    \"queryGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Category or group the detecting query belongs to\"\n    },\n    \"languageName\": {\n      \"type\": \"string\",\n      \"description\": \"Programming language of the scanned source code\"\n    },\n    \"vulnerabilityDetails\": {\n      \"$ref\": \"#/$defs/VulnerabilityDetails\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/Location\"\n    },\n    \"codeFlow\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CodeFlowNode\"\n      },\n      \"description\": \"Ordered list of code flow nodes showing the data flow path from source to sink (SAST findings)\"\n    },\n    \"packageData\"\
  : {\n      \"$ref\": \"#/$defs/PackageData\"\n    },\n    \"firstFoundAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this finding was first detected\"\n    },\n    \"foundAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this finding was detected in the current scan\"\n    },\n    \"comments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Comment\"\n      },\n      \"description\": \"Triage comments added by security reviewers\"\n    }\n  },\n  \"$defs\": {\n    \"VulnerabilityDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed vulnerability classification and scoring information\",\n      \"properties\": {\n        \"cweId\": {\n          \"type\": \"integer\",\n          \"description\": \"Common Weakness Enumeration identifier\"\n        },\n        \"cvss\": {\n          \"type\": \"number\",\n    \
  \      \"format\": \"float\",\n          \"minimum\": 0,\n          \"maximum\": 10,\n          \"description\": \"Common Vulnerability Scoring System score\"\n        },\n        \"cveName\": {\n          \"type\": \"string\",\n          \"pattern\": \"^CVE-\\\\d{4}-\\\\d{4,}$\",\n          \"description\": \"CVE identifier if applicable\"\n        },\n        \"compliances\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Compliance standards this finding relates to (e.g., OWASP Top 10, PCI DSS)\"\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Vulnerability categories\"\n        }\n      }\n    },\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\": \"Source code location where the finding was detected\",\n      \"properties\": {\n        \"fileName\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Source file path\"\n        },\n        \"line\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Line number in the source file\"\n        },\n        \"column\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Column number in the source line\"\n        },\n        \"fullName\": {\n          \"type\": \"string\",\n          \"description\": \"Fully qualified name of the element containing the finding\"\n        }\n      }\n    },\n    \"CodeFlowNode\": {\n      \"type\": \"object\",\n      \"description\": \"A node in the data flow path showing how tainted data travels through the code\",\n      \"properties\": {\n        \"fileName\": {\n          \"type\": \"string\",\n          \"description\": \"Source file name\"\n        },\n        \"line\": {\n          \"type\": \"integer\",\n          \"description\": \"Line number\"\n\
  \        },\n        \"column\": {\n          \"type\": \"integer\",\n          \"description\": \"Column number\"\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"description\": \"Length of the code element\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Node name or code element\"\n        },\n        \"fullName\": {\n          \"type\": \"string\",\n          \"description\": \"Fully qualified name\"\n        },\n        \"methodLine\": {\n          \"type\": \"integer\",\n          \"description\": \"Starting line of the containing method\"\n        }\n      }\n    },\n    \"PackageData\": {\n      \"type\": \"object\",\n      \"description\": \"Open source package information for SCA findings\",\n      \"properties\": {\n        \"packageIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"Package ecosystem and name identifier\"\n        },\n        \"packageName\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"Package name\"\n        },\n        \"packageVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Detected package version\"\n        },\n        \"packageRepository\": {\n          \"type\": \"string\",\n          \"description\": \"Package ecosystem (npm, maven, nuget, pypi, etc.)\"\n        },\n        \"recommendedVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Recommended version that fixes the vulnerability\"\n        },\n        \"isDirectDependency\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the package is a direct dependency or transitive\"\n        }\n      }\n    },\n    \"Comment\": {\n      \"type\": \"object\",\n      \"description\": \"A triage comment added to a finding\",\n      \"properties\": {\n        \"comment\": {\n          \"type\": \"string\",\n          \"description\": \"Comment text\"\n        },\n        \"createdBy\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"User who created the comment\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Comment creation timestamp\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/json-schema/checkmarx-scan-result-schema.json
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
title: Checkmarx Scan Result
---
