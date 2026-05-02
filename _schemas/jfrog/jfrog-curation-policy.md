---
description: Represents a curation policy in JFrog Curation that automatically vets and blocks malicious, vulnerable, or risky open-source packages before they enter the development environment. Curation acts as a gateway between public package registries and internal repositories.
layout: schema
name: JFrog Curation Policy
properties_list:
- description: Unique name identifying the curation policy
  name: policy_name
  type: string
- description: Human-readable description of the policy purpose
  name: description
  type: string
- description: Whether the policy is actively enforced
  name: enabled
  type: boolean
- description: Type of curation policy defining its behavior
  name: policy_type
  type: string
- description: Remote repository keys this policy applies to
  name: repositories
  type: array
- description: Package ecosystem types this policy applies to
  name: package_types
  type: array
- description: Conditions that trigger the policy action
  name: conditions
  type: object
- description: Actions taken when policy conditions are met
  name: actions
  type: object
- description: Policy creation timestamp
  name: created
  type: string
- description: Last modification timestamp
  name: modified
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-curation-policy-schema.json
slug: jfrog-curation-policy
source_filename: jfrog-curation-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/curation-policy\",\n  \"title\": \"JFrog Curation Policy\",\n  \"description\": \"Represents a curation policy in JFrog Curation that automatically vets and blocks malicious, vulnerable, or risky open-source packages before they enter the development environment. Curation acts as a gateway between public package registries and internal repositories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name identifying the curation policy\",\n      \"examples\": [\n        \"block-critical-vulnerabilities\",\n        \"require-license-approval\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the policy purpose\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy\
  \ is actively enforced\",\n      \"default\": true\n    },\n    \"policy_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of curation policy defining its behavior\",\n      \"enum\": [\n        \"block_malicious_packages\",\n        \"block_packages_with_vulnerabilities\",\n        \"block_packages_without_license\",\n        \"block_packages_by_name\",\n        \"block_packages_by_age\",\n        \"allow_only_approved_packages\",\n        \"custom\"\n      ]\n    },\n    \"repositories\": {\n      \"type\": \"array\",\n      \"description\": \"Remote repository keys this policy applies to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"package_types\": {\n      \"type\": \"array\",\n      \"description\": \"Package ecosystem types this policy applies to\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"npm\",\n          \"maven\",\n          \"pypi\",\n          \"docker\",\n          \"go\",\n   \
  \       \"nuget\",\n          \"gems\",\n          \"cargo\",\n          \"conda\",\n          \"composer\",\n          \"helm\"\n        ]\n      }\n    },\n    \"conditions\": {\n      \"type\": \"object\",\n      \"description\": \"Conditions that trigger the policy action\",\n      \"properties\": {\n        \"min_severity\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum vulnerability severity to trigger blocking\",\n          \"enum\": [\n            \"Low\",\n            \"Medium\",\n            \"High\",\n            \"Critical\"\n          ]\n        },\n        \"max_age_days\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum package age in days (for age-based blocking)\",\n          \"minimum\": 1\n        },\n        \"banned_package_names\": {\n          \"type\": \"array\",\n          \"description\": \"Specific package names to block\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n\
  \        \"banned_licenses\": {\n          \"type\": \"array\",\n          \"description\": \"License types to block\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"approved_packages\": {\n          \"type\": \"array\",\n          \"description\": \"Explicitly approved packages (for allow-list policies)\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"version\": {\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        }\n      }\n    },\n    \"actions\": {\n      \"type\": \"object\",\n      \"description\": \"Actions taken when policy conditions are met\",\n      \"properties\": {\n        \"block\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to block the package\
  \ download\"\n        },\n        \"notify\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to send notifications\"\n        },\n        \"notify_emails\": {\n          \"type\": \"array\",\n          \"description\": \"Email addresses to notify\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          }\n        },\n        \"custom_message\": {\n          \"type\": \"string\",\n          \"description\": \"Custom message returned to the user when a package is blocked\"\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Policy creation timestamp\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"required\": [\n    \"policy_name\",\n    \"policy_type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-curation-policy-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Curation Policy
---
