---
description: A PSIRT security advisory for a Palo Alto Networks product.
layout: schema
name: Advisory
properties_list:
- description: Palo Alto Networks advisory identifier (e.g., PAN-SA-2024-0001).
  name: advisory_id
  type: string
- description: CVE identifier (e.g., CVE-2024-3400).
  name: cve_id
  type: string
- description: Advisory title summarizing the vulnerability.
  name: title
  type: string
- description: Detailed description of the vulnerability including impact and attack vector.
  name: description
  type: string
- description: Severity rating based on CVSS v3.1 base score.
  name: severity
  type: string
- description: CVSS v3.1 base score (0.0 to 10.0).
  name: cvss_score
  type: number
- description: CVSS v3.1 vector string (e.g., CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H).
  name: cvss_vector
  type: string
- description: CWE identifier for the vulnerability class.
  name: cwe
  type: string
- description: Products and version ranges affected by this vulnerability.
  name: affected_products
  type: array
- description: Product versions in which the vulnerability is fixed.
  name: fixed_versions
  type: array
- description: Available workarounds or mitigations if a fix is not yet deployed.
  name: workarounds
  type: string
- description: Known exploit activity status.
  name: exploit_status
  type: string
- description: Date and time when the advisory was first published.
  name: published_date
  type: string
- description: Date and time of the most recent advisory update.
  name: last_modified_date
  type: string
- description: External references and related advisories.
  name: references
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/security-advisory-api-advisory-schema.json
slug: security-advisory-api-advisory
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Advisory\",\n  \"description\": \"A PSIRT security advisory for a Palo Alto Networks product.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/security-advisory-api-advisory-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"advisory_id\": {\n      \"type\": \"string\",\n      \"description\": \"Palo Alto Networks advisory identifier (e.g., PAN-SA-2024-0001).\"\n    },\n    \"cve_id\": {\n      \"type\": \"string\",\n      \"description\": \"CVE identifier (e.g., CVE-2024-3400).\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Advisory title summarizing the vulnerability.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the vulnerability including impact and attack vector.\"\n    },\n    \"severity\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ],\n      \"description\": \"Severity rating based on CVSS v3.1 base score.\"\n    },\n    \"cvss_score\": {\n      \"type\": \"number\",\n      \"description\": \"CVSS v3.1 base score (0.0 to 10.0).\",\n      \"minimum\": 0.0,\n      \"maximum\": 10.0\n    },\n    \"cvss_vector\": {\n      \"type\": \"string\",\n      \"description\": \"CVSS v3.1 vector string (e.g., CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H).\"\n    },\n    \"cwe\": {\n      \"type\": \"string\",\n      \"description\": \"CWE identifier for the vulnerability class.\"\n    },\n    \"affected_products\": {\n      \"type\": \"array\",\n      \"description\": \"Products and version ranges affected by this vulnerability.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Product name (e.g., PAN-OS, Cortex XDR Agent).\"\n          },\n          \"versions\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"version\": {\n                  \"type\": \"string\",\n                  \"description\": \"Affected version or version range.\"\n                },\n                \"status\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"Affected\",\n                    \"Unaffected\",\n                    \"Fixed\"\n                  ],\n                  \"description\": \"Vulnerability status for this version.\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"fixed_versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Product versions in which the vulnerability is fixed.\"\n    },\n  \
  \  \"workarounds\": {\n      \"type\": \"string\",\n      \"description\": \"Available workarounds or mitigations if a fix is not yet deployed.\"\n    },\n    \"exploit_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"None\",\n        \"Proof-of-Concept\",\n        \"Active\"\n      ],\n      \"description\": \"Known exploit activity status.\"\n    },\n    \"published_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the advisory was first published.\"\n    },\n    \"last_modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the most recent advisory update.\"\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Reference URL.\"\
  \n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the referenced resource.\"\n          }\n        }\n      },\n      \"description\": \"External references and related advisories.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/security-advisory-api-advisory-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Advisory
---
