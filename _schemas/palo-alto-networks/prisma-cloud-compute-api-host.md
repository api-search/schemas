---
description: Host schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: Host
properties_list:
- description: Unique host identifier.
  name: _id
  type: string
- description: Host machine hostname.
  name: hostname
  type: string
- description: Timestamp of the most recent host scan.
  name: scanTime
  type: string
- description: Operating system distribution.
  name: osDistro
  type: string
- description: Operating system version.
  name: osDistroVersion
  type: string
- description: Linux kernel version.
  name: kernelVersion
  type: string
- description: Cloud provider metadata for the host.
  name: cloudMetadata
  type: object
- description: Vulnerabilities discovered on the host.
  name: vulnerabilities
  type: array
- description: Total number of vulnerabilities found.
  name: vulnerabilitiesCount
  type: integer
- description: ''
  name: vulnerabilityDistribution
  type: object
- description: ''
  name: complianceIssues
  type: array
- description: ''
  name: complianceIssuesCount
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-host-schema.json
slug: prisma-cloud-compute-api-host
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Host\",\n  \"description\": \"Host schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-host-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique host identifier.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Host machine hostname.\"\n    },\n    \"scanTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent host scan.\"\n    },\n    \"osDistro\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system distribution.\"\n    },\n    \"osDistroVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system version.\"\n    },\n\
  \    \"kernelVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Linux kernel version.\"\n    },\n    \"cloudMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Cloud provider metadata for the host.\",\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"aws\",\n            \"azure\",\n            \"gcp\",\n            \"oci\"\n          ]\n        },\n        \"accountId\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n        },\n        \"instanceId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"vulnerabilities\": {\n      \"type\": \"array\",\n      \"description\": \"Vulnerabilities discovered on the host.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"CVE identifier (e.g., CVE-2024-1234).\"\
  \n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"fixed in\",\n              \"needed\",\n              \"will not fix\",\n              \"deferred\"\n            ],\n            \"description\": \"Fix availability status.\"\n          },\n          \"cvss\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"description\": \"CVSS v3 base score.\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"critical\",\n              \"high\",\n              \"medium\",\n              \"low\"\n            ],\n            \"description\": \"Severity level derived from CVSS score.\"\n          },\n          \"packageName\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the affected package.\"\n          },\n          \"packageVersion\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Installed version of the affected package.\"\n          },\n          \"fixedVersion\": {\n            \"type\": \"string\",\n            \"description\": \"Version that contains the fix, if available.\"\n          },\n          \"link\": {\n            \"type\": \"string\",\n            \"description\": \"URL to the CVE advisory or details page.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Brief description of the vulnerability.\"\n          },\n          \"publishedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Date the vulnerability was publicly disclosed.\"\n          }\n        }\n      }\n    },\n    \"vulnerabilitiesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of vulnerabilities found.\"\n    },\n    \"vulnerabilityDistribution\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"critical\"\
  : {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"complianceIssues\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"Compliance check ID.\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"Title of the compliance check.\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"critical\",\n              \"high\",\n              \"medium\",\n              \"low\"\n            ],\n            \"description\": \"Severity of the compliance issue.\"\n          },\n          \"cause\": {\n            \"type\": \"\
  string\",\n            \"description\": \"Explanation of why the resource failed the check.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Detailed description of the compliance requirement.\"\n          }\n        }\n      }\n    },\n    \"complianceIssuesCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-host-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Host
---
