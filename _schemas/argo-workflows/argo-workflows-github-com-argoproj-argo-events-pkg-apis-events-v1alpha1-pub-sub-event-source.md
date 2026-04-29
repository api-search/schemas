---
description: PubSubEventSource refers to event-source for GCP PubSub related events.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PubSubEventSource
properties_list:
- description: ''
  name: credentialSecret
  type: object
- description: ''
  name: deleteSubscriptionOnFinish
  type: boolean
- description: ''
  name: filter
  type: object
- description: ''
  name: jsonBody
  type: boolean
- description: ''
  name: metadata
  type: object
- description: ''
  name: projectID
  type: string
- description: ''
  name: subscriptionID
  type: string
- description: ''
  name: topic
  type: string
- description: ''
  name: topicProjectID
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pub-sub-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pub-sub-event-source
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pub-sub-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pub-sub-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PubSubEventSource\",\n  \"description\": \"PubSubEventSource refers to event-source for GCP PubSub related events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"credentialSecret\": {\n      \"title\": \"CredentialSecret references to the secret that contains JSON credentials to access GCP.\\nIf it is missing, it implicitly uses Workload Identity to access.\\nhttps://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"deleteSubscriptionOnFinish\": {\n      \"type\": \"boolean\",\n      \"title\": \"DeleteSubscriptionOnFinish\
  \ determines whether to delete the GCP PubSub subscription once the event source is stopped.\\n+optional\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\n    },\n    \"jsonBody\": {\n      \"type\": \"boolean\",\n      \"title\": \"JSONBody specifies that all event body payload coming from this\\nsource will be JSON\\n+optional\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"projectID\": {\n      \"type\": \"string\",\n      \"title\": \"ProjectID is GCP project ID for the subscription.\\nRequired if you run Argo Events outside of GKE/GCE.\\n(otherwise, the default value is its project)\\n+optional\"\n    },\n    \"subscriptionID\": {\n  \
  \    \"type\": \"string\",\n      \"title\": \"SubscriptionID is ID of subscription.\\nRequired if you use existing subscription.\\nThe default value will be auto generated hash based on this eventsource setting, so the subscription\\nmight be recreated every time you update the setting, which has a possibility of event loss.\\n+optional\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"title\": \"Topic to which the subscription should belongs.\\nRequired if you want the eventsource to create a new subscription.\\nIf you specify this field along with an existing subscription,\\nit will be verified whether it actually belongs to the specified topic.\\n+optional\"\n    },\n    \"topicProjectID\": {\n      \"type\": \"string\",\n      \"title\": \"TopicProjectID is GCP project ID for the topic.\\nBy default, it is same as ProjectID.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-pub-sub-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PubSubEventSource
---
