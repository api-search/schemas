---
description: A Common Vulnerabilities and Exposures record from the Red Hat Security Data API
layout: schema
name: RHEL CVE
properties_list:
- description: CVE identifier
  name: name
  type: string
- description: Red Hat severity rating
  name: threat_severity
  type: string
- description: Date the CVE was made public
  name: public_date
  type: string
- description: Associated Bugzilla ticket
  name: bugzilla
  type: object
- description: CVSS v2 scoring information
  name: cvss
  type: object
- description: CVSS v3 scoring information
  name: cvss3
  type: object
- description: CWE identifier
  name: cwe
  type: string
- description: Detailed description of the vulnerability
  name: details
  type: array
- description: Red Hat impact statement
  name: statement
  type: string
- description: Fixed package releases
  name: affected_release
  type: array
- description: Packages without an available fix
  name: package_state
  type: array
provider_name: Red Hat Enterprise Linux
provider_slug: rhel
schema_file: json-schema/rhel-cve-schema.json
slug: rhel-cve
source_filename: rhel-cve-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/rhel/blob/main/json-schema/rhel-cve-schema.json\",\n  \"title\": \"RHEL CVE\",\n  \"description\": \"A Common Vulnerabilities and Exposures record from the Red Hat Security Data API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"CVE identifier\",\n      \"pattern\": \"^CVE-\\\\d{4}-\\\\d{4,}$\",\n      \"example\": \"CVE-2021-23358\"\n    },\n    \"threat_severity\": {\n      \"type\": \"string\",\n      \"description\": \"Red Hat severity rating\",\n      \"enum\": [\"Low\", \"Moderate\", \"Important\", \"Critical\"]\n    },\n    \"public_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the CVE was made public\"\n    },\n    \"bugzilla\": {\n      \"type\": \"object\",\n      \"description\": \"Associated Bugzilla ticket\",\n      \"properties\"\
  : {\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"cvss\": {\n      \"type\": \"object\",\n      \"description\": \"CVSS v2 scoring information\",\n      \"properties\": {\n        \"cvss_base_score\": {\n          \"type\": \"string\"\n        },\n        \"cvss_scoring_vector\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"cvss3\": {\n      \"type\": \"object\",\n      \"description\": \"CVSS v3 scoring information\",\n      \"properties\": {\n        \"cvss3_base_score\": {\n          \"type\": \"string\"\n        },\n        \"cvss3_scoring_vector\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"cwe\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"CWE identifier\",\n      \"example\": \"CWE-77\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Detailed description of the vulnerability\"\n    },\n    \"statement\": {\n      \"type\": \"string\",\n      \"description\": \"Red Hat impact statement\"\n    },\n    \"affected_release\": {\n      \"type\": \"array\",\n      \"description\": \"Fixed package releases\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product_name\": {\n            \"type\": \"string\"\n          },\n          \"release_date\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"advisory\": {\n            \"type\": \"string\"\n          },\n          \"cpe\": {\n            \"type\": \"string\"\n          },\n          \"package\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    },\n    \"package_state\": {\n      \"type\": \"array\",\n      \"description\": \"Packages without an available fix\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"product_name\": {\n            \"type\": \"string\"\n          },\n          \"fix_state\": {\n            \"type\": \"string\",\n            \"enum\": [\"Affected\", \"Will not fix\", \"Fix deferred\", \"Not affected\", \"Out of support scope\"]\n          },\n          \"package_name\": {\n            \"type\": \"string\"\n          },\n          \"cpe\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"threat_severity\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/json-schema/rhel-cve-schema.json
tags:
- Automation
- Compliance
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
- Security
- Subscription Management
- Vulnerability Management
title: RHEL CVE
---
