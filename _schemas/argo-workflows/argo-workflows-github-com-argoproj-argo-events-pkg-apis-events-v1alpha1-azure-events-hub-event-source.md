---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventsHubEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventsHubEventSource
properties_list:
- description: ''
  name: filter
  type: object
- description: ''
  name: fqdn
  type: string
- description: ''
  name: hubName
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: sharedAccessKey
  type: object
- description: ''
  name: sharedAccessKeyName
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-events-hub-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-events-hub-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-events-hub-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventsHubEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventsHubEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"title\": \"FQDN of the EventHubs namespace you created\\nMore info at https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-get-connection-string\"\n    },\n    \"hubName\"\
  : {\n      \"type\": \"string\",\n      \"title\": \"Event Hub path/name\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sharedAccessKey\": {\n      \"title\": \"SharedAccessKey is the generated value of the key. If both this field and SharedAccessKeyName are not provided\\nit will try to access via Azure AD with DefaultAzureCredential, FQDN and HubName.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"sharedAccessKeyName\": {\n      \"title\": \"SharedAccessKeyName is the name you chose for your application's SAS keys. If both this field and SharedAccessKey are not provided\\nit will try to access via Azure AD with DefaultAzureCredential, FQDN and HubName.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-azure-events-hub-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventsHubEventSource
---
