---
description: Schema for a Red Hat advisory (erratum) representing a security fix, bug fix, or enhancement update applicable to registered RHEL systems through the Insights Patch service.
layout: schema
name: Red Hat Insights Advisory
properties_list:
- description: The advisory identifier in Red Hat format (e.g., RHSA-2024:1234, RHBA-2024:5678).
  name: id
  type: string
- description: The type of advisory indicating the nature of the update.
  name: type
  type: string
- description: A brief summary of the advisory content.
  name: synopsis
  type: string
- description: A detailed description of the advisory including affected components and changes.
  name: description
  type: string
- description: The severity rating for security advisories, null for non-security advisories.
  name: severity
  type:
  - string
  - 'null'
- description: The date and time the advisory was publicly released.
  name: public_date
  type: string
- description: The date and time the advisory was last modified.
  name: modified_date
  type: string
- description: The number of registered systems to which this advisory is applicable.
  name: applicable_systems
  type: integer
- description: The list of CVE identifiers addressed by this advisory.
  name: cves
  type: array
- description: The list of updated package names included in the advisory.
  name: packages
  type: array
- description: External references related to the advisory.
  name: references
  type: array
- description: Whether applying this advisory requires a system reboot.
  name: reboot_required
  type: boolean
- description: The RHEL release versions this advisory applies to.
  name: release_versions
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-advisory-schema.json
slug: red-hat-insights-advisory
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://console.redhat.com/schemas/red-hat/insights-advisory.json\",\n  \"title\": \"Red Hat Insights Advisory\",\n  \"description\": \"Schema for a Red Hat advisory (erratum) representing a security fix, bug fix, or enhancement update applicable to registered RHEL systems through the Insights Patch service.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"synopsis\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The advisory identifier in Red Hat format (e.g., RHSA-2024:1234, RHBA-2024:5678).\",\n      \"pattern\": \"^RH[SBEA]A-\\\\d{4}:\\\\d+$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of advisory indicating the nature of the update.\",\n      \"enum\": [\"security\", \"bugfix\", \"enhancement\"]\n    },\n    \"synopsis\": {\n      \"type\": \"string\",\n      \"description\": \"A brief\
  \ summary of the advisory content.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the advisory including affected components and changes.\"\n    },\n    \"severity\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The severity rating for security advisories, null for non-security advisories.\",\n      \"enum\": [\"Critical\", \"Important\", \"Moderate\", \"Low\", null]\n    },\n    \"public_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the advisory was publicly released.\"\n    },\n    \"modified_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the advisory was last modified.\"\n    },\n    \"applicable_systems\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of registered systems to which this advisory is applicable.\",\n      \"minimum\"\
  : 0\n    },\n    \"cves\": {\n      \"type\": \"array\",\n      \"description\": \"The list of CVE identifiers addressed by this advisory.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^CVE-\\\\d{4}-\\\\d+$\",\n        \"description\": \"A CVE identifier.\"\n      }\n    },\n    \"packages\": {\n      \"type\": \"array\",\n      \"description\": \"The list of updated package names included in the advisory.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Package\"\n      }\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"description\": \"External references related to the advisory.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The reference type.\",\n            \"enum\": [\"bugzilla\", \"cve\", \"self\", \"other\"]\n          },\n          \"href\": {\n            \"type\": \"string\",\n            \"format\"\
  : \"uri\",\n            \"description\": \"The URL of the reference.\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The reference identifier.\"\n          }\n        }\n      }\n    },\n    \"reboot_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether applying this advisory requires a system reboot.\",\n      \"default\": false\n    },\n    \"release_versions\": {\n      \"type\": \"array\",\n      \"description\": \"The RHEL release versions this advisory applies to.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"A RHEL release version string.\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Package\": {\n      \"type\": \"object\",\n      \"description\": \"An RPM package included in the advisory update.\",\n      \"required\": [\"name\", \"evra\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The package name.\"\
  \n        },\n        \"evra\": {\n          \"type\": \"string\",\n          \"description\": \"The epoch:version-release.arch string of the updated package.\"\n        },\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"A brief summary of the package.\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": \"RHSA-2024:1234\",\n      \"type\": \"security\",\n      \"synopsis\": \"Important: kernel security and bug fix update\",\n      \"description\": \"An update for kernel is now available for Red Hat Enterprise Linux 9. Red Hat Product Security has rated this update as having a security impact of Important.\",\n      \"severity\": \"Important\",\n      \"public_date\": \"2024-06-15T14:00:00Z\",\n      \"modified_date\": \"2024-06-16T10:00:00Z\",\n      \"applicable_systems\": 42,\n      \"cves\": [\n        \"CVE-2024-1234\",\n        \"CVE-2024-5678\"\n      ],\n      \"packages\": [\n        {\n          \"name\": \"kernel\"\
  ,\n          \"evra\": \"0:5.14.0-362.18.1.el9_3.x86_64\",\n          \"summary\": \"The Linux kernel\"\n        }\n      ],\n      \"reboot_required\": true,\n      \"release_versions\": [\"9.3\"]\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-advisory-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Red Hat Insights Advisory
---
