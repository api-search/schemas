---
description: Schema for a compliance control mapped to one or more regulatory frameworks, as used by compliance automation platforms.
layout: schema
name: Compliance Control
properties_list:
- description: Unique identifier for the compliance control.
  name: controlId
  type: string
- description: Short name or title of the control.
  name: name
  type: string
- description: Detailed description of what the control requires.
  name: description
  type: string
- description: Compliance domain this control falls under (e.g., 'Access Control', 'Encryption', 'Incident Response').
  name: domain
  type: string
- description: Compliance frameworks this control satisfies.
  name: frameworks
  type: array
- description: Guidance on how to implement this control.
  name: implementationGuidance
  type: string
- description: Types of evidence that can satisfy this control (e.g., 'Screenshot', 'Policy Document', 'Log Export', 'API Integration').
  name: evidenceTypes
  type: array
- description: Whether evidence collection for this control can be automated via API integration.
  name: automatable
  type: boolean
- description: Current implementation status.
  name: status
  type: string
- description: Team or individual responsible for this control.
  name: owner
  type: string
- description: Tags for categorization.
  name: tags
  type: array
provider_name: Regulatory Templates
provider_slug: regulatory-templates
schema_file: json-schema/regulatory-templates-control-schema.json
slug: regulatory-templates-control
source_filename: regulatory-templates-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regulatory-templates/json-schema/regulatory-templates-control-schema.json\",\n  \"title\": \"Compliance Control\",\n  \"description\": \"Schema for a compliance control mapped to one or more regulatory frameworks, as used by compliance automation platforms.\",\n  \"type\": \"object\",\n  \"required\": [\"controlId\", \"name\", \"domain\", \"frameworks\"],\n  \"properties\": {\n    \"controlId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the compliance control.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Short name or title of the control.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of what the control requires.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance domain this control\
  \ falls under (e.g., 'Access Control', 'Encryption', 'Incident Response').\"\n    },\n    \"frameworks\": {\n      \"type\": \"array\",\n      \"description\": \"Compliance frameworks this control satisfies.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"frameworkId\", \"controlReference\"],\n        \"properties\": {\n          \"frameworkId\": {\n            \"type\": \"string\",\n            \"description\": \"Framework identifier (e.g., 'SOC2', 'ISO27001', 'HIPAA', 'GDPR', 'PCIDSS').\",\n            \"enum\": [\"SOC2\", \"ISO27001\", \"HIPAA\", \"GDPR\", \"PCIDSS\", \"CCPA\", \"NIST CSF\", \"FedRAMP\", \"CMMC\", \"CIS Controls\"]\n          },\n          \"controlReference\": {\n            \"type\": \"string\",\n            \"description\": \"Framework-specific control reference (e.g., 'CC6.1', 'A.9.4.1', '164.312(a)(1)').\"\n          },\n          \"requirementText\": {\n            \"type\": \"string\",\n            \"description\": \"The verbatim\
  \ requirement text from the framework.\"\n          }\n        }\n      }\n    },\n    \"implementationGuidance\": {\n      \"type\": \"string\",\n      \"description\": \"Guidance on how to implement this control.\"\n    },\n    \"evidenceTypes\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Types of evidence that can satisfy this control (e.g., 'Screenshot', 'Policy Document', 'Log Export', 'API Integration').\"\n    },\n    \"automatable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether evidence collection for this control can be automated via API integration.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current implementation status.\",\n      \"enum\": [\"Not Started\", \"In Progress\", \"Implemented\", \"Needs Review\", \"Failing\"]\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Team or individual responsible for this control.\"\n    },\n\
  \    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Tags for categorization.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regulatory-templates/refs/heads/main/json-schema/regulatory-templates-control-schema.json
tags:
- Compliance
- Governance
- GDPR
- HIPAA
- ISO 27001
- PCI DSS
- Policy Templates
- Regulatory
- SOC 2
- Templates
title: Compliance Control
---
