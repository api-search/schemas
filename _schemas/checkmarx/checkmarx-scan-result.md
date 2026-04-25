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
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
title: Checkmarx Scan Result
---
