---
description: A CVE (Common Vulnerabilities and Exposures) record from the NIST National Vulnerability Database
layout: schema
name: NVD CVE Record
properties_list:
- description: CVE identifier
  name: id
  type: string
- description: CNA (CVE Numbering Authority) that assigned the CVE
  name: sourceIdentifier
  type: string
- description: Date the CVE was published in NVD
  name: published
  type: string
- description: ''
  name: lastModified
  type: string
- description: ''
  name: vulnStatus
  type: string
- description: ''
  name: descriptions
  type: array
- description: ''
  name: metrics
  type: object
- description: ''
  name: weaknesses
  type: array
- description: ''
  name: configurations
  type: array
- description: ''
  name: references
  type: array
- description: Date added to CISA Known Exploited Vulnerabilities catalog
  name: cisaExploitAdd
  type:
  - string
  - 'null'
- description: ''
  name: cisaActionDue
  type:
  - string
  - 'null'
- description: ''
  name: cisaRequiredAction
  type:
  - string
  - 'null'
- description: ''
  name: cisaVulnerabilityName
  type:
  - string
  - 'null'
provider_name: NVD
provider_slug: nvd
schema_file: json-schema/nvd-cve-schema.json
slug: nvd-cve
source_filename: nvd-cve-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/json-schema/nvd-cve-schema.json\",\n  \"title\": \"NVD CVE Record\",\n  \"description\": \"A CVE (Common Vulnerabilities and Exposures) record from the NIST National Vulnerability Database\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"published\", \"lastModified\", \"vulnStatus\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"CVE identifier\",\n      \"pattern\": \"^CVE-[0-9]{4}-[0-9]{4,}$\"\n    },\n    \"sourceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"CNA (CVE Numbering Authority) that assigned the CVE\"\n    },\n    \"published\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the CVE was published in NVD\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  \n    },\n    \"vulnStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Analyzed\", \"Awaiting Analysis\", \"Undergoing Analysis\", \"Modified\", \"Deferred\", \"Rejected\", \"Received\"]\n    },\n    \"descriptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"lang\", \"value\"],\n        \"properties\": {\n          \"lang\": { \"type\": \"string\", \"description\": \"ISO 639-1 language code\" },\n          \"value\": { \"type\": \"string\", \"description\": \"CVE description text\" }\n        }\n      }\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cvssMetricV31\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/CVSSMetricV3\" }\n        },\n        \"cvssMetricV30\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/CVSSMetricV3\" }\n        },\n        \"cvssMetricV2\": {\n          \"type\": \"array\",\n\
  \          \"items\": { \"$ref\": \"#/$defs/CVSSMetricV2\" }\n        }\n      }\n    },\n    \"weaknesses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"source\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\" },\n          \"description\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"lang\": { \"type\": \"string\" },\n                \"value\": { \"type\": \"string\", \"description\": \"CWE ID (e.g., CWE-79)\" }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"configurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"nodes\": {\n            \"type\": \"array\",\n            \"items\": { \"$ref\": \"#/$defs/ConfigNode\" }\n          }\n        }\n      }\n    },\n    \"references\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n          \"source\": { \"type\": \"string\" },\n          \"tags\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          }\n        }\n      }\n    },\n    \"cisaExploitAdd\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date added to CISA Known Exploited Vulnerabilities catalog\"\n    },\n    \"cisaActionDue\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\"\n    },\n    \"cisaRequiredAction\": {\n      \"type\": [\"string\", \"null\"]\n    },\n    \"cisaVulnerabilityName\": {\n      \"type\": [\"string\", \"null\"]\n    }\n  },\n  \"$defs\": {\n    \"CVSSMetricV3\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"source\": { \"type\": \"string\" },\n        \"type\": { \"\
  type\": \"string\", \"enum\": [\"Primary\", \"Secondary\"] },\n        \"cvssData\": {\n          \"type\": \"object\",\n          \"required\": [\"version\", \"vectorString\", \"baseScore\", \"baseSeverity\"],\n          \"properties\": {\n            \"version\": { \"type\": \"string\", \"enum\": [\"3.0\", \"3.1\"] },\n            \"vectorString\": { \"type\": \"string\" },\n            \"attackVector\": { \"type\": \"string\", \"enum\": [\"NETWORK\", \"ADJACENT_NETWORK\", \"LOCAL\", \"PHYSICAL\"] },\n            \"attackComplexity\": { \"type\": \"string\", \"enum\": [\"LOW\", \"HIGH\"] },\n            \"privilegesRequired\": { \"type\": \"string\", \"enum\": [\"NONE\", \"LOW\", \"HIGH\"] },\n            \"userInteraction\": { \"type\": \"string\", \"enum\": [\"NONE\", \"REQUIRED\"] },\n            \"scope\": { \"type\": \"string\", \"enum\": [\"UNCHANGED\", \"CHANGED\"] },\n            \"confidentialityImpact\": { \"type\": \"string\", \"enum\": [\"NONE\", \"LOW\", \"HIGH\"] },\n \
  \           \"integrityImpact\": { \"type\": \"string\", \"enum\": [\"NONE\", \"LOW\", \"HIGH\"] },\n            \"availabilityImpact\": { \"type\": \"string\", \"enum\": [\"NONE\", \"LOW\", \"HIGH\"] },\n            \"baseScore\": { \"type\": \"number\", \"minimum\": 0, \"maximum\": 10 },\n            \"baseSeverity\": { \"type\": \"string\", \"enum\": [\"NONE\", \"LOW\", \"MEDIUM\", \"HIGH\", \"CRITICAL\"] }\n          }\n        },\n        \"exploitabilityScore\": { \"type\": \"number\", \"minimum\": 0, \"maximum\": 10 },\n        \"impactScore\": { \"type\": \"number\", \"minimum\": 0, \"maximum\": 10 }\n      }\n    },\n    \"CVSSMetricV2\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"source\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\", \"enum\": [\"Primary\", \"Secondary\"] },\n        \"cvssData\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"version\": { \"type\": \"string\", \"enum\": [\"2.0\"\
  ] },\n            \"vectorString\": { \"type\": \"string\" },\n            \"baseScore\": { \"type\": \"number\", \"minimum\": 0, \"maximum\": 10 }\n          }\n        },\n        \"baseSeverity\": { \"type\": \"string\", \"enum\": [\"LOW\", \"MEDIUM\", \"HIGH\"] }\n      }\n    },\n    \"ConfigNode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"operator\": { \"type\": \"string\", \"enum\": [\"AND\", \"OR\"] },\n        \"negate\": { \"type\": \"boolean\" },\n        \"cpeMatch\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"vulnerable\": { \"type\": \"boolean\" },\n              \"criteria\": { \"type\": \"string\", \"description\": \"CPE 2.3 name string\" },\n              \"matchCriteriaId\": { \"type\": \"string\", \"format\": \"uuid\" },\n              \"versionStartIncluding\": { \"type\": \"string\" },\n              \"versionStartExcluding\": { \"type\": \"string\"\
  \ },\n              \"versionEndIncluding\": { \"type\": \"string\" },\n              \"versionEndExcluding\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/json-schema/nvd-cve-schema.json
tags:
- Security
- CVE
- CPE
- Vulnerability
- CVSS
title: NVD CVE Record
---
