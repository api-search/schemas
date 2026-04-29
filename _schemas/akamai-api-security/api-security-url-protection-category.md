---
description: Specify one or more load shedding categories for the URL protection policy.
layout: schema
name: url-protection-category
properties_list:
- description: Specify the type of traffic to shed first before reaching the requests per second (RPS) limit. `BOTS` includes bots from Akamai's existing list of known bots. `CLIENT_REPUTATIONS` includes traffic fro
  name: type
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-url-protection-category-schema.json
slug: api-security-url-protection-category
source_filename: api-security-url-protection-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-category-schema.json\",\n  \"title\": \"url-protection-category\",\n  \"description\": \"Specify one or more load shedding categories for the URL protection policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"Specify the type of traffic to shed first before reaching the requests per second (RPS) limit. `BOTS` includes bots from Akamai's existing list of known bots. `CLIENT_REPUTATIONS` includes traffic from clients with a bad client reputation score. `CLOUD_PROVIDERS` includes traffic from providers like AWS, Microsoft Azure, and Google Cloud. `PROXIES` includes proxy traffic as determined by IPQualityScore (IPQS) and Akamai EdgeScape. `TOR_EXIT_NODES` includes traffic defined in Akamai's existing network list of nodes. `PLATFORM_DDOS_INTELLIGENCE`\
  \ includes traffic detected by Akamai's DDOS Intelligence platform.\",\n      \"enum\": [\n        \"BOTS\",\n        \"CLIENT_REPUTATIONS\",\n        \"CLOUD_PROVIDERS\",\n        \"PROXIES\",\n        \"TOR_EXIT_NODES\",\n        \"PLATFORM_DDOS_INTELLIGENCE\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-category-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: url-protection-category
---
