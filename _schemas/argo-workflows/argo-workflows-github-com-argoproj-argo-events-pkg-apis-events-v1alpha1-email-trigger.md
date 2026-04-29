---
description: EmailTrigger refers to the specification of the email notification trigger.
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EmailTrigger
properties_list:
- description: ''
  name: body
  type: string
- description: ''
  name: from
  type: string
- description: Host refers to the smtp host url to which email is send.
  name: host
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: port
  type: integer
- description: ''
  name: smtpPassword
  type: object
- description: ''
  name: subject
  type: string
- description: ''
  name: to
  type: array
- description: ''
  name: username
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-email-trigger-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-email-trigger
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-email-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-email-trigger-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EmailTrigger\",\n  \"description\": \"EmailTrigger refers to the specification of the email notification trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\",\n      \"title\": \"Body refers to the body/content of the email send.\\n+optional\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"title\": \"From refers to the address from which the email is send from.\\n+optional\"\n    },\n    \"host\": {\n      \"description\": \"Host refers to the smtp host url to which email is send.\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\"\
  ,\n      \"title\": \"Parameters is the list of key-value extracted from event's payload that are applied to\\nthe trigger resource.\\n+optional\",\n      \"items\": {\n        \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.TriggerParameter\"\n      }\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"title\": \"Port refers to the smtp server port to which email is send.\\nDefaults to 0.\\n+optional\"\n    },\n    \"smtpPassword\": {\n      \"title\": \"SMTPPassword refers to the Kubernetes secret that holds the smtp password used to connect to smtp server.\\n+optional\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"title\": \"Subject refers to the subject line for the email send.\\n+optional\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"title\": \"To refers to the email addresses to which the emails are send.\\n+optional\",\n   \
  \   \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username refers to the username used to connect to the smtp server.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-email-trigger-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EmailTrigger
---
