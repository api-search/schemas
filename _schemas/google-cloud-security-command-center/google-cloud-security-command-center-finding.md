---
description: Schema for a Security Command Center finding, representing a security issue or threat detected in a cloud resource.
layout: schema
name: Google Cloud Security Command Center Finding
properties_list:
- description: The relative resource name of the finding
  name: name
  type: string
- description: The relative resource name of the source the finding belongs to
  name: parent
  type: string
- description: The state of the finding
  name: state
  type: string
- description: The additional taxonomy group within findings from a given source
  name: category
  type: string
- description: The full resource name of the Google Cloud resource this finding is for
  name: resourceName
  type: string
- description: The severity of the finding
  name: severity
  type: string
- description: URI that points to a web page with additional information about the finding
  name: externalUri
  type: string
- description: Source-specific properties that are set by the source that writes the finding
  name: sourceProperties
  type: object
- description: The time the finding was first detected
  name: eventTime
  type: string
- description: The time at which the finding was created in Security Command Center
  name: createTime
  type: string
- description: User-specified security marks applied to the finding
  name: securityMarks
  type: object
- description: Represents vulnerability-specific fields like CVE and CVSS scores
  name: vulnerability
  type: object
provider_name: Google Cloud Security Command Center
provider_slug: google-cloud-security-command-center
schema_file: json-schema/google-cloud-security-command-center-finding-schema.json
slug: google-cloud-security-command-center-finding
source_filename: google-cloud-security-command-center-finding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/securitycenter/finding.json\",\n  \"title\": \"Google Cloud Security Command Center Finding\",\n  \"description\": \"Schema for a Security Command Center finding, representing a security issue or threat detected in a cloud resource.\",\n  \"type\": \"object\",\n  \"required\": [\"category\", \"resourceName\", \"state\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The relative resource name of the finding\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The relative resource name of the source the finding belongs to\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the finding\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\"]\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The additional taxonomy group\
  \ within findings from a given source\"\n    },\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The full resource name of the Google Cloud resource this finding is for\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity of the finding\",\n      \"enum\": [\"CRITICAL\", \"HIGH\", \"MEDIUM\", \"LOW\"]\n    },\n    \"externalUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URI that points to a web page with additional information about the finding\"\n    },\n    \"sourceProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Source-specific properties that are set by the source that writes the finding\",\n      \"additionalProperties\": true\n    },\n    \"eventTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the finding was first detected\"\n    },\n    \"createTime\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"The time at which the finding was created in Security Command Center\"\n    },\n    \"securityMarks\": {\n      \"$ref\": \"#/$defs/SecurityMarks\",\n      \"description\": \"User-specified security marks applied to the finding\"\n    },\n    \"vulnerability\": {\n      \"$ref\": \"#/$defs/Vulnerability\",\n      \"description\": \"Represents vulnerability-specific fields like CVE and CVSS scores\"\n    }\n  },\n  \"$defs\": {\n    \"SecurityMarks\": {\n      \"type\": \"object\",\n      \"description\": \"User-specified security marks attached to the finding\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The relative resource name of the SecurityMarks\"\n        },\n        \"marks\": {\n          \"type\": \"object\",\n          \"description\": \"Mutable user-specified security marks\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    },\n    \"Vulnerability\": {\n      \"type\": \"object\",\n      \"description\": \"Vulnerability information for the finding\",\n      \"properties\": {\n        \"cve\": {\n          \"type\": \"object\",\n          \"description\": \"CVE information\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The unique CVE identifier\"\n            },\n            \"cvssv3\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"baseScore\": {\n                  \"type\": \"number\",\n                  \"description\": \"The base score for CVSS v3\"\n                },\n                \"attackVector\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"NETWORK\", \"ADJACENT\", \"LOCAL\", \"PHYSICAL\"]\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-security-command-center/refs/heads/main/json-schema/google-cloud-security-command-center-finding-schema.json
tags:
- Cloud Security
- Compliance
- Risk Management
- Security
- Threat Detection
- Vulnerability Management
title: Google Cloud Security Command Center Finding
---
