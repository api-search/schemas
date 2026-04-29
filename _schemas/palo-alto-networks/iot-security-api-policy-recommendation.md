---
description: PolicyRecommendation schema from Palo Alto Networks IoT Security API
layout: schema
name: PolicyRecommendation
properties_list:
- description: Unique recommendation identifier.
  name: id
  type: string
- description: Device identifier the recommendation applies to.
  name: deviceid
  type: string
- description: Device profile the recommendation applies to.
  name: profile
  type: string
- description: Recommended source security zone.
  name: source_zone
  type: string
- description: Recommended destination security zone.
  name: destination_zone
  type: string
- description: Recommended allowed applications.
  name: applications
  type: array
- description: Recommended allowed services and ports.
  name: services
  type: array
- description: Recommended policy action.
  name: action
  type: string
- description: Confidence score for the recommendation.
  name: confidence
  type: number
- description: Human-readable recommendation description.
  name: description
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/iot-security-api-policy-recommendation-schema.json
slug: iot-security-api-policy-recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyRecommendation\",\n  \"description\": \"PolicyRecommendation schema from Palo Alto Networks IoT Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-policy-recommendation-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique recommendation identifier.\"\n    },\n    \"deviceid\": {\n      \"type\": \"string\",\n      \"description\": \"Device identifier the recommendation applies to.\"\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"description\": \"Device profile the recommendation applies to.\"\n    },\n    \"source_zone\": {\n      \"type\": \"string\",\n      \"description\": \"Recommended source security zone.\"\n    },\n    \"destination_zone\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Recommended destination security zone.\"\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Recommended allowed applications.\"\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Recommended allowed services and ports.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"deny\",\n        \"alert\"\n      ],\n      \"description\": \"Recommended policy action.\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Confidence score for the recommendation.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable recommendation description.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-policy-recommendation-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PolicyRecommendation
---
