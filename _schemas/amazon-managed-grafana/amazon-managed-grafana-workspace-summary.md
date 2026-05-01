---
description: A structure that contains some information about one workspace in the account.
layout: schema
name: WorkspaceSummary
properties_list:
- description: ''
  name: authentication
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: endpoint
  type: object
- description: ''
  name: grafanaVersion
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: modified
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: notificationDestinations
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-workspace-summary-schema.json
slug: amazon-managed-grafana-workspace-summary
source_filename: amazon-managed-grafana-workspace-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-workspace-summary-schema.json\",\n  \"title\": \"WorkspaceSummary\",\n  \"description\": \"A structure that contains some information about one workspace in the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationSummary\"\n        },\n        {\n          \"description\": \"A structure containing information about the authentication methods used in the workspace.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date that the workspace was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The customer-entered description of the workspace.\"\n        }\n      ]\n    },\n    \"endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Endpoint\"\n        },\n        {\n          \"description\": \"The URL endpoint to use to access the Grafana console in the workspace.\"\n        }\n      ]\n    },\n    \"grafanaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrafanaVersion\"\n        },\n        {\n          \"description\": \"The Grafana version that the workspace is running.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The unique ID of the workspace.\"\n        }\n      ]\n    },\n    \"modified\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The most recent date that the workspace was modified.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceName\"\n        },\n        {\n          \"description\": \"The name of the workspace.\"\n        }\n      ]\n    },\n    \"notificationDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationDestinationsList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services notification channels that Amazon Managed Grafana can automatically create IAM roles and permissions for, which allows Amazon Managed Grafana to use these channels.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceStatus\"\n        },\n        {\n          \"description\": \"The current\
  \ status of the workspace.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of tags associated with the workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"authentication\",\n    \"created\",\n    \"endpoint\",\n    \"grafanaVersion\",\n    \"id\",\n    \"modified\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-workspace-summary-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: WorkspaceSummary
---
