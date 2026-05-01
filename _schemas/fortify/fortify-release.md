---
description: Represents a release (version) of an application in the Fortify platform. Releases track the security posture of a specific version of an application through its development lifecycle, aggregating scan results and vulnerability metrics.
layout: schema
name: Fortify Release
properties_list:
- description: Unique identifier of the release
  name: releaseId
  type: integer
- description: Name of the release
  name: releaseName
  type: string
- description: Description of the release
  name: releaseDescription
  type: string
- description: Identifier of the parent application
  name: applicationId
  type: integer
- description: Name of the parent application
  name: applicationName
  type: string
- description: Software development lifecycle status
  name: sdlcStatusType
  type: string
- description: Security rating for the release (0-5 stars)
  name: rating
  type: number
- description: Number of critical severity issues
  name: critical
  type: integer
- description: Number of high severity issues
  name: high
  type: integer
- description: Number of medium severity issues
  name: medium
  type: integer
- description: Number of low severity issues
  name: low
  type: integer
- description: Total number of open issues
  name: issueCount
  type: integer
- description: Whether the release passes the security policy
  name: isPassed
  type: boolean
- description: Reason for the pass or fail status
  name: passFailReasonType
  type: string
- description: Identifier of the most recent static scan
  name: currentStaticScanId
  type: integer
- description: Identifier of the most recent dynamic scan
  name: currentDynamicScanId
  type: integer
- description: Identifier of the most recent mobile scan
  name: currentMobileScanId
  type: integer
- description: Optional microservice identifier if this release belongs to a microservice
  name: microserviceId
  type: integer
- description: Name of the associated microservice
  name: microserviceName
  type: string
provider_name: Fortify
provider_slug: fortify
schema_file: json-schema/fortify-release-schema.json
slug: fortify-release
source_filename: fortify-release-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/fortify/json-schema/fortify-release-schema.json\",\n  \"title\": \"Fortify Release\",\n  \"description\": \"Represents a release (version) of an application in the Fortify platform. Releases track the security posture of a specific version of an application through its development lifecycle, aggregating scan results and vulnerability metrics.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"releaseName\"\n  ],\n  \"properties\": {\n    \"releaseId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Unique identifier of the release\"\n    },\n    \"releaseName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the release\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"releaseDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the release\"\n    },\n\
  \    \"applicationId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Identifier of the parent application\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent application\"\n    },\n    \"sdlcStatusType\": {\n      \"type\": \"string\",\n      \"description\": \"Software development lifecycle status\",\n      \"enum\": [\n        \"Development\",\n        \"QA\",\n        \"Production\",\n        \"Retired\"\n      ]\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Security rating for the release (0-5 stars)\",\n      \"minimum\": 0,\n      \"maximum\": 5\n    },\n    \"critical\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of critical severity issues\",\n      \"minimum\": 0\n    },\n    \"high\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\"\
  : \"Number of high severity issues\",\n      \"minimum\": 0\n    },\n    \"medium\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of medium severity issues\",\n      \"minimum\": 0\n    },\n    \"low\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of low severity issues\",\n      \"minimum\": 0\n    },\n    \"issueCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Total number of open issues\",\n      \"minimum\": 0\n    },\n    \"isPassed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the release passes the security policy\"\n    },\n    \"passFailReasonType\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the pass or fail status\"\n    },\n    \"currentStaticScanId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Identifier of the most recent static scan\"\
  \n    },\n    \"currentDynamicScanId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Identifier of the most recent dynamic scan\"\n    },\n    \"currentMobileScanId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Identifier of the most recent mobile scan\"\n    },\n    \"microserviceId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Optional microservice identifier if this release belongs to a microservice\"\n    },\n    \"microserviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the associated microservice\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/json-schema/fortify-release-schema.json
tags:
- Application Security
- DAST
- DevSecOps
- SAST
- SCA
- Security Testing
- Vulnerability Scanning
title: Fortify Release
---
