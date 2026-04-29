---
description: Image schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: Image
properties_list:
- description: Unique image identifier composed of registry, repository, and tag.
  name: _id
  type: string
- description: Hostname of the machine where the image was scanned.
  name: hostname
  type: string
- description: Timestamp of the most recent scan.
  name: scanTime
  type: string
- description: Repository and tag information for the image.
  name: repoTag
  type: object
- description: Content-addressable image digests.
  name: repoDigests
  type: array
- description: Operating system distribution of the image.
  name: osDistro
  type: string
- description: Operating system distribution version.
  name: osDistroVersion
  type: string
- description: Vulnerabilities discovered in the image.
  name: vulnerabilities
  type: array
- description: Total number of vulnerabilities found.
  name: vulnerabilitiesCount
  type: integer
- description: Vulnerability count by severity level.
  name: vulnerabilityDistribution
  type: object
- description: Compliance check failures for the image.
  name: complianceIssues
  type: array
- description: Total number of compliance issues found.
  name: complianceIssuesCount
  type: integer
- description: Kubernetes clusters where this image is deployed.
  name: clusters
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-image-schema.json
slug: prisma-cloud-compute-api-image
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Image\",\n  \"description\": \"Image schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-image-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique image identifier composed of registry, repository, and tag.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the machine where the image was scanned.\"\n    },\n    \"scanTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent scan.\"\n    },\n    \"repoTag\": {\n      \"type\": \"object\",\n      \"description\": \"Repository and tag information for the image.\",\n      \"properties\": {\n        \"registry\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Container registry URL.\"\n        },\n        \"repo\": {\n          \"type\": \"string\",\n          \"description\": \"Repository name.\"\n        },\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"Image tag.\"\n        }\n      }\n    },\n    \"repoDigests\": {\n      \"type\": \"array\",\n      \"description\": \"Content-addressable image digests.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"osDistro\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system distribution of the image.\"\n    },\n    \"osDistroVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system distribution version.\"\n    },\n    \"vulnerabilities\": {\n      \"type\": \"array\",\n      \"description\": \"Vulnerabilities discovered in the image.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n     \
  \     \"id\": {\n            \"type\": \"string\",\n            \"description\": \"CVE identifier (e.g., CVE-2024-1234).\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"fixed in\",\n              \"needed\",\n              \"will not fix\",\n              \"deferred\"\n            ],\n            \"description\": \"Fix availability status.\"\n          },\n          \"cvss\": {\n            \"type\": \"number\",\n            \"format\": \"float\",\n            \"description\": \"CVSS v3 base score.\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"critical\",\n              \"high\",\n              \"medium\",\n              \"low\"\n            ],\n            \"description\": \"Severity level derived from CVSS score.\"\n          },\n          \"packageName\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the affected\
  \ package.\"\n          },\n          \"packageVersion\": {\n            \"type\": \"string\",\n            \"description\": \"Installed version of the affected package.\"\n          },\n          \"fixedVersion\": {\n            \"type\": \"string\",\n            \"description\": \"Version that contains the fix, if available.\"\n          },\n          \"link\": {\n            \"type\": \"string\",\n            \"description\": \"URL to the CVE advisory or details page.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Brief description of the vulnerability.\"\n          },\n          \"publishedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Date the vulnerability was publicly disclosed.\"\n          }\n        }\n      }\n    },\n    \"vulnerabilitiesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of vulnerabilities found.\"\
  \n    },\n    \"vulnerabilityDistribution\": {\n      \"type\": \"object\",\n      \"description\": \"Vulnerability count by severity level.\",\n      \"properties\": {\n        \"critical\": {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"complianceIssues\": {\n      \"type\": \"array\",\n      \"description\": \"Compliance check failures for the image.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"Compliance check ID.\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"Title of the compliance check.\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"\
  enum\": [\n              \"critical\",\n              \"high\",\n              \"medium\",\n              \"low\"\n            ],\n            \"description\": \"Severity of the compliance issue.\"\n          },\n          \"cause\": {\n            \"type\": \"string\",\n            \"description\": \"Explanation of why the resource failed the check.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Detailed description of the compliance requirement.\"\n          }\n        }\n      }\n    },\n    \"complianceIssuesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of compliance issues found.\"\n    },\n    \"clusters\": {\n      \"type\": \"array\",\n      \"description\": \"Kubernetes clusters where this image is deployed.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-image-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Image
---
