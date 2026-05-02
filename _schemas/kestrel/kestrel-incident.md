---
description: Represents a cloud or Kubernetes infrastructure incident detected, investigated, and remediated by the Kestrel AI platform.
layout: schema
name: Kestrel Incident
properties_list:
- description: Unique identifier for the incident.
  name: incidentId
  type: string
- description: Human-readable summary of the incident.
  name: name
  type: string
- description: Detailed description of the incident including symptoms and impact.
  name: description
  type: string
- description: Severity level of the incident.
  name: severity
  type: string
- description: Current status of the incident in the response lifecycle.
  name: status
  type: string
- description: The Kubernetes cluster where the incident was detected.
  name: cluster
  type: object
- description: Kubernetes namespace where the incident occurred.
  name: namespace
  type: string
- description: AI-determined root cause analysis of the incident.
  name: rootCause
  type: string
- description: Kubernetes resources affected by this incident.
  name: affectedResources
  type: array
- description: Details of the automated remediation applied.
  name: remediation
  type: object
- description: Timestamp when the incident was first detected.
  name: detectedAt
  type: string
- description: Timestamp when the incident was resolved.
  name: resolvedAt
  type: string
- description: Categorization tags for the incident.
  name: tags
  type: array
provider_name: Kestrel
provider_slug: kestrel
schema_file: json-schema/kestrel-incident-schema.json
slug: kestrel-incident
source_filename: kestrel-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://usekestrel.ai/schemas/kestrel/incident.json\",\n  \"title\": \"Kestrel Incident\",\n  \"description\": \"Represents a cloud or Kubernetes infrastructure incident detected, investigated, and remediated by the Kestrel AI platform.\",\n  \"type\": \"object\",\n  \"required\": [\"incidentId\", \"name\", \"severity\", \"status\"],\n  \"properties\": {\n    \"incidentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the incident.\",\n      \"pattern\": \"^inc_.+\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable summary of the incident.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the incident including symptoms and impact.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level\
  \ of the incident.\",\n      \"enum\": [\"critical\", \"high\", \"medium\", \"low\", \"info\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the incident in the response lifecycle.\",\n      \"enum\": [\"detected\", \"investigating\", \"remediating\", \"resolved\", \"closed\"]\n    },\n    \"cluster\": {\n      \"$ref\": \"#/$defs/ClusterRef\",\n      \"description\": \"The Kubernetes cluster where the incident was detected.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace where the incident occurred.\"\n    },\n    \"rootCause\": {\n      \"type\": \"string\",\n      \"description\": \"AI-determined root cause analysis of the incident.\"\n    },\n    \"affectedResources\": {\n      \"type\": \"array\",\n      \"description\": \"Kubernetes resources affected by this incident.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AffectedResource\"\n      }\n    },\n    \"remediation\"\
  : {\n      \"$ref\": \"#/$defs/Remediation\",\n      \"description\": \"Details of the automated remediation applied.\"\n    },\n    \"detectedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the incident was first detected.\",\n      \"format\": \"date-time\"\n    },\n    \"resolvedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the incident was resolved.\",\n      \"format\": \"date-time\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Categorization tags for the incident.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ClusterRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Kubernetes cluster monitored by Kestrel.\",\n      \"properties\": {\n        \"clusterId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the cluster.\"\n        },\n        \"name\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Name of the Kubernetes cluster.\"\n        },\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider hosting the cluster.\",\n          \"enum\": [\"aws\", \"gcp\", \"azure\", \"on-premise\", \"other\"]\n        }\n      },\n      \"required\": [\"clusterId\", \"name\"]\n    },\n    \"AffectedResource\": {\n      \"type\": \"object\",\n      \"description\": \"A Kubernetes resource affected by an incident.\",\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes resource kind (e.g., Pod, Deployment, Service).\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the Kubernetes resource.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the resource.\"\n        }\n      },\n      \"required\": [\"kind\", \"name\"]\n\
  \    },\n    \"Remediation\": {\n      \"type\": \"object\",\n      \"description\": \"Automated remediation details produced by Kestrel AI agents.\",\n      \"properties\": {\n        \"remediationId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the remediation action.\",\n          \"pattern\": \"^rem_.+\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the remediation action taken.\"\n        },\n        \"pullRequestUrl\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the pull request containing the fix.\",\n          \"format\": \"uri\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the remediation.\",\n          \"enum\": [\"proposed\", \"approved\", \"applied\", \"reverted\", \"failed\"]\n        },\n        \"appliedAt\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Timestamp when the remediation was applied.\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kestrel/refs/heads/main/json-schema/kestrel-incident-schema.json
tags:
- AI Agents
- Cloud Security
- Incident Response
- Kubernetes
- Observability
title: Kestrel Incident
---
