---
description: A Mule application deployed to CloudHub. Contains metadata about the application configuration, deployment status, worker settings, and runtime properties.
layout: schema
name: Application
properties_list:
- description: Unique domain name for the application, used as the subdomain in the CloudHub URL (e.g., myapp.cloudhub.io)
  name: domain
  type: string
- description: Full domain including the cloudhub.io suffix
  name: fullDomain
  type: string
- description: Current deployment status of the application
  name: status
  type: string
- description: Human-readable description of the application
  name: description
  type: string
- description: CloudHub region where the application is deployed
  name: region
  type: string
- description: Mule runtime version information
  name: muleVersion
  type: object
- description: Application properties passed to the Mule runtime
  name: properties
  type: object
- description: Unix timestamp of the last application update
  name: lastUpdateTime
  type: integer
- description: Name of the deployed application archive file
  name: fileName
  type: string
- description: Whether Anypoint Monitoring is enabled for this application
  name: monitoringEnabled
  type: boolean
- description: Whether automatic restart on failure is enabled
  name: monitoringAutoRestart
  type: boolean
- description: Whether static IPs are allocated to this application
  name: staticIPsEnabled
  type: boolean
- description: Whether persistent queues are enabled
  name: persistentQueues
  type: boolean
- description: Whether persistent queue data is encrypted
  name: persistentQueuesEncrypted
  type: boolean
- description: Whether the application uses Object Store v1
  name: objectStoreV1
  type: boolean
- description: Whether next-generation logging is enabled
  name: loggingNgEnabled
  type: boolean
- description: Transaction tracking configuration
  name: trackingSettings
  type: object
- description: ID of the VPN if the application is connected to one
  name: vpnId
  type: string
- description: VPN configuration for the application
  name: vpnConfig
  type: object
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-application-schema.json
slug: mulesoft-anypoint-platform-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"description\": \"A Mule application deployed to CloudHub. Contains metadata about the application configuration, deployment status, worker settings, and runtime properties.\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Unique domain name for the application, used as the subdomain in the CloudHub URL (e.g., myapp.cloudhub.io)\"\n    },\n    \"fullDomain\": {\n      \"type\": \"string\",\n      \"description\": \"Full domain including the cloudhub.io suffix\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current deployment status of the application\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the application\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"\
  CloudHub region where the application is deployed\"\n    },\n    \"muleVersion\": {\n      \"type\": \"object\",\n      \"description\": \"Mule runtime version information\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Application properties passed to the Mule runtime\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the last application update\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the deployed application archive file\"\n    },\n    \"monitoringEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Anypoint Monitoring is enabled for this application\"\n    },\n    \"monitoringAutoRestart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether automatic restart on failure is enabled\"\n    },\n    \"staticIPsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether static IPs are\
  \ allocated to this application\"\n    },\n    \"persistentQueues\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether persistent queues are enabled\"\n    },\n    \"persistentQueuesEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether persistent queue data is encrypted\"\n    },\n    \"objectStoreV1\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application uses Object Store v1\"\n    },\n    \"loggingNgEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether next-generation logging is enabled\"\n    },\n    \"trackingSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Transaction tracking configuration\"\n    },\n    \"vpnId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the VPN if the application is connected to one\"\n    },\n    \"vpnConfig\": {\n      \"type\": \"object\",\n      \"description\": \"VPN configuration for the application\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-application-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: Application
---
