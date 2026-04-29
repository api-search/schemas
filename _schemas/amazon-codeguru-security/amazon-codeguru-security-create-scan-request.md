---
description: CreateScanRequest schema from Amazon CodeGuru Security
layout: schema
name: CreateScanRequest
properties_list:
- description: ''
  name: analysisType
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: scanName
  type: object
- description: ''
  name: scanType
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-create-scan-request-schema.json
slug: amazon-codeguru-security-create-scan-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-scan-request-schema.json\",\n  \"title\": \"CreateScanRequest\",\n  \"description\": \"CreateScanRequest schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analysisType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisType\"\n        },\n        {\n          \"description\": \"The type of analysis you want CodeGuru Security to perform in the scan, either <code>Security</code> or <code>All</code>. The <code>Security</code> type only generates findings related to security. The <code>All</code> type generates both security findings and quality findings. Defaults to <code>Security</code> type if missing.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token for the request. Amazon CodeGuru Security uses this value to prevent the accidental creation of duplicate scans if there are failures and retries.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for an input resource used to create a scan.\"\n        }\n      ]\n    },\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanName\"\n        },\n        {\n          \"description\": \"The unique name that CodeGuru Security uses to track revisions across multiple scans of the same resource. Only allowed for a <code>STANDARD</code> scan type. If not specified, it will be auto generated. \"\n        }\n      ]\n    },\n    \"scanType\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ScanType\"\n        },\n        {\n          \"description\": \"<p>The type of scan, either <code>Standard</code> or <code>Express</code>. Defaults to <code>Standard</code> type if missing.</p> <p> <code>Express</code> scans run on limited resources and use a limited set of detectors to analyze your code in near-real time. <code>Standard</code> scans have standard resource limits and use the full set of detectors to analyze your code.</p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>An array of key-value pairs used to tag a scan. A tag is a custom attribute label with two parts:</p> <ul> <li> <p>A tag key. For example, <code>CostCenter</code>, <code>Environment</code>, or <code>Secret</code>. Tag keys are case sensitive.</p> </li> <li> <p>An optional tag value field. For example, <code>111122223333</code>,\
  \ <code>Production</code>, or a team name. Omitting the tag value is the same as using an empty string. Tag values are case sensitive.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceId\",\n    \"scanName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-scan-request-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: CreateScanRequest
---
