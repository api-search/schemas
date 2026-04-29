---
description: TriggerTemplate is the template that describes trigger specification.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerTemplate
properties_list:
- description: ''
  name: argoWorkflow
  type: object
- description: ''
  name: awsLambda
  type: object
- description: ''
  name: azureEventHubs
  type: object
- description: ''
  name: azureServiceBus
  type: object
- description: ''
  name: conditions
  type: string
- description: ''
  name: conditionsReset
  type: array
- description: ''
  name: custom
  type: object
- description: ''
  name: email
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: k8s
  type: object
- description: Kafka refers to the trigger designed to place messages on Kafka topic. +optional.
  name: kafka
  type: object
- description: ''
  name: log
  type: object
- description: Name is a unique name of the action to take.
  name: name
  type: string
- description: NATS refers to the trigger designed to place message on NATS subject. +optional.
  name: nats
  type: object
- description: ''
  name: openWhisk
  type: object
- description: ''
  name: pulsar
  type: object
- description: ''
  name: slack
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerTemplate\",\n  \"description\": \"TriggerTemplate is the template that describes trigger specification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"argoWorkflow\": {\n      \"title\": \"ArgoWorkflow refers to the trigger that can perform various operations on an Argo io.argoproj.workflow.v1alpha1.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArgoWorkflowTrigger\"\n    },\n    \"awsLambda\": {\n      \"title\": \"AWSLambda refers to the trigger designed to invoke AWS Lambda function with with on-the-fly constructable payload.\\n+optional\",\n      \"$ref\"\
  : \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AWSLambdaTrigger\"\n    },\n    \"azureEventHubs\": {\n      \"title\": \"AzureEventHubs refers to the trigger send an event to an Azure Event Hub.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureEventHubsTrigger\"\n    },\n    \"azureServiceBus\": {\n      \"title\": \"AzureServiceBus refers to the trigger designed to place messages on Azure Service Bus\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.AzureServiceBusTrigger\"\n    },\n    \"conditions\": {\n      \"type\": \"string\",\n      \"title\": \"Conditions is the conditions to execute the trigger.\\nFor example: \\\"(dep01 || dep02) && dep04\\\"\\n+optional\"\n    },\n    \"conditionsReset\": {\n      \"type\": \"array\",\n      \"title\": \"Criteria to reset the conditons\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ConditionsResetCriteria\"\
  \n      }\n    },\n    \"custom\": {\n      \"title\": \"CustomTrigger refers to the trigger designed to connect to a gRPC trigger server and execute a custom trigger.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.CustomTrigger\"\n    },\n    \"email\": {\n      \"title\": \"Email refers to the trigger designed to send an email notification\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EmailTrigger\"\n    },\n    \"http\": {\n      \"title\": \"HTTP refers to the trigger designed to dispatch a HTTP request with on-the-fly constructable payload.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HTTPTrigger\"\n    },\n    \"k8s\": {\n      \"title\": \"StandardK8STrigger refers to the trigger designed to create or update a generic Kubernetes resource.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.StandardK8STrigger\"\
  \n    },\n    \"kafka\": {\n      \"description\": \"Kafka refers to the trigger designed to place messages on Kafka topic.\\n+optional.\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.KafkaTrigger\"\n    },\n    \"log\": {\n      \"title\": \"Log refers to the trigger designed to invoke log the io.argoproj.workflow.v1alpha1.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.LogTrigger\"\n    },\n    \"name\": {\n      \"description\": \"Name is a unique name of the action to take.\",\n      \"type\": \"string\"\n    },\n    \"nats\": {\n      \"description\": \"NATS refers to the trigger designed to place message on NATS subject.\\n+optional.\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.NATSTrigger\"\n    },\n    \"openWhisk\": {\n      \"title\": \"OpenWhisk refers to the trigger designed to invoke OpenWhisk action.\\n+optional\",\n     \
  \ \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.OpenWhiskTrigger\"\n    },\n    \"pulsar\": {\n      \"title\": \"Pulsar refers to the trigger designed to place messages on Pulsar topic.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.PulsarTrigger\"\n    },\n    \"slack\": {\n      \"title\": \"Slack refers to the trigger designed to send slack notification message.\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.SlackTrigger\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-trigger-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerTemplate
---
