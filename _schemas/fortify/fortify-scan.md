---
description: Represents a security scan performed by Fortify tools. Scans analyze applications for vulnerabilities using static analysis (SAST), dynamic analysis (DAST), mobile testing, or software composition analysis. Each scan produces vulnerability findings associated with a release.
layout: schema
name: Fortify Scan
properties_list:
- description: Unique identifier of the scan
  name: scanId
  type: integer
- description: Type of security scan performed
  name: scanType
  type: string
- description: Current analysis status of the scan
  name: analysisStatusType
  type: string
- description: Identifier of the associated release
  name: releaseId
  type: integer
- description: Identifier of the associated application
  name: applicationId
  type: integer
- description: Assessment type used for the scan
  name: assessmentTypeId
  type: integer
- description: Entitlement used for the scan
  name: entitlementId
  type: integer
- description: Date and time when the scan started
  name: startedDateTime
  type: string
- description: Date and time when the scan completed
  name: completedDateTime
  type: string
- description: Total number of vulnerability issues found
  name: totalIssues
  type: integer
- description: Number of critical severity issues found
  name: issueCountCritical
  type: integer
- description: Number of high severity issues found
  name: issueCountHigh
  type: integer
- description: Number of medium severity issues found
  name: issueCountMedium
  type: integer
- description: Number of low severity issues found
  name: issueCountLow
  type: integer
- description: Whether this scan is a remediation verification scan
  name: isRemediationScan
  type: boolean
- description: Whether this scan used a bundled assessment
  name: isBundledAssessment
  type: boolean
- description: Whether the scan passes the configured security policy
  name: passFailStatus
  type: boolean
- description: Reason for the pass or fail determination
  name: passFailReasonType
  type: string
- description: Technology stack analyzed (for static scans)
  name: technologyStack
  type: string
- description: Language level used for analysis (for static scans)
  name: languageLevel
  type: string
provider_name: Fortify
provider_slug: fortify
schema_file: json-schema/fortify-scan-schema.json
slug: fortify-scan
source_filename: fortify-scan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/fortify/json-schema/fortify-scan-schema.json\",\n  \"title\": \"Fortify Scan\",\n  \"description\": \"Represents a security scan performed by Fortify tools. Scans analyze applications for vulnerabilities using static analysis (SAST), dynamic analysis (DAST), mobile testing, or software composition analysis. Each scan produces vulnerability findings associated with a release.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scanId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Unique identifier of the scan\"\n    },\n    \"scanType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of security scan performed\",\n      \"enum\": [\n        \"Static\",\n        \"Dynamic\",\n        \"Mobile\",\n        \"OpenSource\"\n      ]\n    },\n    \"analysisStatusType\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Current analysis status of the scan\"\n    },\n    \"releaseId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Identifier of the associated release\"\n    },\n    \"applicationId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Identifier of the associated application\"\n    },\n    \"assessmentTypeId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Assessment type used for the scan\"\n    },\n    \"entitlementId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Entitlement used for the scan\"\n    },\n    \"startedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the scan started\"\n    },\n    \"completedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the scan\
  \ completed\"\n    },\n    \"totalIssues\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Total number of vulnerability issues found\",\n      \"minimum\": 0\n    },\n    \"issueCountCritical\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of critical severity issues found\",\n      \"minimum\": 0\n    },\n    \"issueCountHigh\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of high severity issues found\",\n      \"minimum\": 0\n    },\n    \"issueCountMedium\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of medium severity issues found\",\n      \"minimum\": 0\n    },\n    \"issueCountLow\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of low severity issues found\",\n      \"minimum\": 0\n    },\n    \"isRemediationScan\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether this scan is a remediation verification scan\",\n      \"default\": false\n    },\n    \"isBundledAssessment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this scan used a bundled assessment\",\n      \"default\": false\n    },\n    \"passFailStatus\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the scan passes the configured security policy\"\n    },\n    \"passFailReasonType\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the pass or fail determination\"\n    },\n    \"technologyStack\": {\n      \"type\": \"string\",\n      \"description\": \"Technology stack analyzed (for static scans)\"\n    },\n    \"languageLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Language level used for analysis (for static scans)\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/json-schema/fortify-scan-schema.json
tags:
- Application Security
- DAST
- DevSecOps
- SAST
- SCA
- Security Testing
- Vulnerability Scanning
title: Fortify Scan
---
