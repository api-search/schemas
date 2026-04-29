---
description: An Azure subscription is a logical container used to provision resources in Azure. It holds the details of all your resources like virtual machines (VMs), databases, and more. When you create an Azure resource, you choose the subscription to deploy it to.
layout: schema
name: Azure Subscription
properties_list:
- description: 'The fully qualified ID for the subscription. Format: /subscriptions/{subscriptionId}.'
  name: id
  type: string
- description: The subscription ID.
  name: subscriptionId
  type: string
- description: The subscription display name.
  name: displayName
  type: string
- description: The subscription tenant ID.
  name: tenantId
  type: string
- description: The subscription state. Possible values are Enabled, Warned, PastDue, Disabled, and Deleted.
  name: state
  type: string
- description: The subscription policies.
  name: subscriptionPolicies
  type: object
- description: The authorization source of the request. Valid values are one or more combinations of Legacy, RoleBased, Bypassed, Direct, and Management.
  name: authorizationSource
  type: string
- description: The tags attached to the subscription.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/microsoft-azure-subscription-schema.json
slug: microsoft-azure-subscription
source_filename: microsoft-azure-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-azure/subscription\",\n  \"title\": \"Azure Subscription\",\n  \"description\": \"An Azure subscription is a logical container used to provision resources in Azure. It holds the details of all your resources like virtual machines (VMs), databases, and more. When you create an Azure resource, you choose the subscription to deploy it to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified ID for the subscription. Format: /subscriptions/{subscriptionId}.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"/subscriptions/00000000-0000-0000-0000-000000000000\"\n      ]\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The subscription ID.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"\
  00000000-0000-0000-0000-000000000000\"\n      ]\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription display name.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"My Azure Subscription\",\n        \"Pay-As-You-Go\",\n        \"Visual Studio Enterprise\"\n      ]\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The subscription tenant ID.\",\n      \"readOnly\": true\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription state. Possible values are Enabled, Warned, PastDue, Disabled, and Deleted.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"Enabled\",\n        \"Warned\",\n        \"PastDue\",\n        \"Disabled\",\n        \"Deleted\"\n      ]\n    },\n    \"subscriptionPolicies\": {\n      \"type\": \"object\",\n      \"description\": \"The subscription policies.\",\n      \"properties\": {\n      \
  \  \"locationPlacementId\": {\n          \"type\": \"string\",\n          \"description\": \"The subscription location placement ID. The ID indicates which regions are visible for a subscription.\",\n          \"readOnly\": true\n        },\n        \"quotaId\": {\n          \"type\": \"string\",\n          \"description\": \"The subscription quota ID.\",\n          \"readOnly\": true\n        },\n        \"spendingLimit\": {\n          \"type\": \"string\",\n          \"description\": \"The subscription spending limit.\",\n          \"readOnly\": true,\n          \"enum\": [\n            \"On\",\n            \"Off\",\n            \"CurrentPeriodOff\"\n          ]\n        }\n      }\n    },\n    \"authorizationSource\": {\n      \"type\": \"string\",\n      \"description\": \"The authorization source of the request. Valid values are one or more combinations of Legacy, RoleBased, Bypassed, Direct, and Management.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The tags attached to the subscription.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/microsoft-azure-subscription-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Azure Subscription
---
