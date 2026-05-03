---
description: Schema for a Common Vulnerability and Exposure (CVE) record from the Red Hat Security Data API.
layout: schema
name: Red Hat RHEL CVE
properties_list:
- description: CVE identifier
  name: CVE
  type: string
- description: Red Hat severity rating for this CVE
  name: severity
  type: string
- description: Date the CVE was publicly disclosed
  name: public_date
  type: string
- description: URL to the Red Hat Bugzilla entry for this CVE
  name: bugzilla
  type: string
- description: Description from the Bugzilla entry
  name: bugzilla_description
  type: string
- description: CVSS v2 score
  name: cvss_score
  type: number
- description: CVSS v3 score
  name: cvss3_score
  type: number
- description: Common Weakness Enumeration identifier
  name: cwe
  type: string
- description: Detailed description of the vulnerability
  name: details
  type: array
- description: Credit to those who reported or discovered the vulnerability
  name: acknowledgement
  type: string
- description: List of Red Hat product releases affected by this CVE
  name: affected_release
  type: array
provider_name: Red Hat Enterprise Linux 8
provider_slug: red-hat-enterprise-linux-8
schema_file: json-schema/red-hat-enterprise-linux-8-cve-schema.json
slug: red-hat-enterprise-linux-8-cve
source_filename: red-hat-enterprise-linux-8-cve-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/red-hat-enterprise-linux-8/json-schema/red-hat-enterprise-linux-8-cve-schema.json\",\n  \"title\": \"Red Hat RHEL CVE\",\n  \"description\": \"Schema for a Common Vulnerability and Exposure (CVE) record from the Red Hat Security Data API.\",\n  \"type\": \"object\",\n  \"required\": [\"CVE\", \"severity\"],\n  \"properties\": {\n    \"CVE\": {\n      \"type\": \"string\",\n      \"description\": \"CVE identifier\",\n      \"pattern\": \"^CVE-\\\\d{4}-\\\\d+$\",\n      \"examples\": [\"CVE-2024-1234\"]\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"Critical\", \"Important\", \"Moderate\", \"Low\"],\n      \"description\": \"Red Hat severity rating for this CVE\"\n    },\n    \"public_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the CVE was publicly disclosed\"\n    },\n   \
  \ \"bugzilla\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the Red Hat Bugzilla entry for this CVE\"\n    },\n    \"bugzilla_description\": {\n      \"type\": \"string\",\n      \"description\": \"Description from the Bugzilla entry\"\n    },\n    \"cvss_score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n      \"description\": \"CVSS v2 score\"\n    },\n    \"cvss3_score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n      \"description\": \"CVSS v3 score\"\n    },\n    \"cwe\": {\n      \"type\": \"string\",\n      \"description\": \"Common Weakness Enumeration identifier\",\n      \"pattern\": \"^CWE-\\\\d+$\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed description of the vulnerability\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"acknowledgement\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Credit to those who reported or discovered the vulnerability\"\n    },\n    \"affected_release\": {\n      \"type\": \"array\",\n      \"description\": \"List of Red Hat product releases affected by this CVE\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product_name\": {\n            \"type\": \"string\",\n            \"description\": \"Affected product name\"\n          },\n          \"release_date\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Date the fix was released\"\n          },\n          \"advisory\": {\n            \"type\": \"string\",\n            \"description\": \"Associated Red Hat security advisory ID\"\n          },\n          \"package\": {\n            \"type\": \"string\",\n            \"description\": \"Fixed package name and version (NVR format)\"\n          },\n          \"cpe\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"CPE identifier for the affected product\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-enterprise-linux-8/refs/heads/main/json-schema/red-hat-enterprise-linux-8-cve-schema.json
tags:
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
title: Red Hat RHEL CVE
---
