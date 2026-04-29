---
description: Provider-specific configuration that extends the standard OAuth flow.
layout: schema
name: ProviderAppMetadata
properties_list:
- description: Additional query parameters to include in the OAuth authorization URL (e.g., optional_scope for HubSpot).
  name: authQueryParams
  type: object
- description: Provider-specific string values keyed by names (e.g., packageInstallURL for Salesforce, gcpProjectId and gcpPubSubTopicName for Gmail).
  name: providerParams
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-provider-app-metadata-schema.json
slug: ampersand-api-provider-app-metadata
source_filename: ampersand-api-provider-app-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-provider-app-metadata-schema.json\",\n  \"title\": \"ProviderAppMetadata\",\n  \"description\": \"Provider-specific configuration that extends the standard OAuth flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authQueryParams\": {\n      \"type\": \"object\",\n      \"description\": \"Additional query parameters to include in the OAuth authorization URL (e.g., optional_scope for HubSpot).\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"example\": {\n        \"optional_scope\": [\n          \"automation.sequences.read\"\n        ]\n      }\n    },\n    \"providerParams\": {\n      \"type\": \"object\",\n      \"description\": \"Provider-specific string values keyed by names (e.g.,\
  \ packageInstallURL for Salesforce, gcpProjectId and gcpPubSubTopicName for Gmail).\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"packageInstallURL\": \"https://login.salesforce.com/packaging/installPackage.apexp?p0=04t123456789\",\n        \"gcpProjectId\": \"my-gcp-project\",\n        \"gcpPubSubTopicName\": \"my-topic\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-provider-app-metadata-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ProviderAppMetadata
---
