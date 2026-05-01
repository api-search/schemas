---
description: Schema for the JSON alert output emitted by Falco when a rule is triggered. This is the format used by all Falco output channels including stdout, file, gRPC, and HTTP webhook outputs.
layout: schema
name: Falco Alert Output
properties_list:
- description: Unique identifier for the alert event
  name: uuid
  type: string
- description: Formatted output message as defined by the rule output template
  name: output
  type: string
- description: Severity level of the alert
  name: priority
  type: string
- description: Name of the rule that triggered the alert
  name: rule
  type: string
- description: Data source that generated the event
  name: source
  type: string
- description: ISO 8601 timestamp of when the event occurred
  name: time
  type: string
- description: Hostname of the machine where the event was detected
  name: hostname
  type: string
- description: Tags associated with the triggered rule including MITRE ATT&CK references
  name: tags
  type: array
- description: Key-value pairs of fields extracted from the event
  name: output_fields
  type: object
provider_name: Falco
provider_slug: falco
schema_file: json-schema/falco-alert-output.json
slug: falco-alert-output
source_filename: falco-alert-output.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://falco.org/schemas/output/v1/falco-alert-output.json\",\n  \"title\": \"Falco Alert Output\",\n  \"description\": \"Schema for the JSON alert output emitted by Falco when a rule is triggered. This is the format used by all Falco output channels including stdout, file, gRPC, and HTTP webhook outputs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the alert event\"\n    },\n    \"output\": {\n      \"type\": \"string\",\n      \"description\": \"Formatted output message as defined by the rule output template\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the alert\",\n      \"enum\": [\n        \"Emergency\",\n        \"Alert\",\n        \"Critical\",\n        \"Error\",\n        \"Warning\",\n        \"Notice\"\
  ,\n        \"Informational\",\n        \"Debug\"\n      ]\n    },\n    \"rule\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the rule that triggered the alert\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Data source that generated the event\",\n      \"enum\": [\n        \"syscall\",\n        \"k8s_audit\",\n        \"aws_cloudtrail\",\n        \"okta\",\n        \"github\"\n      ]\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the event occurred\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the machine where the event was detected\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the triggered rule including MITRE ATT&CK references\"\n    },\n    \"output_fields\": {\n  \
  \    \"type\": \"object\",\n      \"description\": \"Key-value pairs of fields extracted from the event\",\n      \"properties\": {\n        \"evt.time\": {\n          \"type\": \"string\",\n          \"description\": \"Event timestamp\"\n        },\n        \"evt.type\": {\n          \"type\": \"string\",\n          \"description\": \"System call or event type\"\n        },\n        \"user.name\": {\n          \"type\": \"string\",\n          \"description\": \"User name associated with the event\"\n        },\n        \"user.uid\": {\n          \"type\": [\"integer\", \"string\"],\n          \"description\": \"User ID associated with the event\"\n        },\n        \"proc.name\": {\n          \"type\": \"string\",\n          \"description\": \"Process name\"\n        },\n        \"proc.pid\": {\n          \"type\": \"integer\",\n          \"description\": \"Process ID\"\n        },\n        \"proc.ppid\": {\n          \"type\": \"integer\",\n          \"description\": \"Parent process\
  \ ID\"\n        },\n        \"proc.cmdline\": {\n          \"type\": \"string\",\n          \"description\": \"Full command line of the process\"\n        },\n        \"proc.pname\": {\n          \"type\": \"string\",\n          \"description\": \"Parent process name\"\n        },\n        \"container.id\": {\n          \"type\": \"string\",\n          \"description\": \"Container ID\"\n        },\n        \"container.name\": {\n          \"type\": \"string\",\n          \"description\": \"Container name\"\n        },\n        \"container.image.repository\": {\n          \"type\": \"string\",\n          \"description\": \"Container image repository\"\n        },\n        \"container.image.tag\": {\n          \"type\": \"string\",\n          \"description\": \"Container image tag\"\n        },\n        \"k8s.ns.name\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace name\"\n        },\n        \"k8s.pod.name\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"Kubernetes pod name\"\n        },\n        \"fd.name\": {\n          \"type\": \"string\",\n          \"description\": \"File descriptor name (file path, connection tuple, etc.)\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": [\"string\", \"integer\", \"boolean\", \"null\"]\n      }\n    }\n  },\n  \"required\": [\"output\", \"priority\", \"rule\", \"source\", \"time\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/falco/refs/heads/main/json-schema/falco-alert-output.json
tags:
- Cloud Native
- eBPF
- Runtime Security
- Security
- Threat Detection
title: Falco Alert Output
---
