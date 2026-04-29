---
description: A structure containing the identity provider (IdP) metadata used to integrate the identity provider with this workspace. You can specify the metadata either by providing a URL to its location in the <code>url</code> parameter, or by specifying the full metadata in XML format in the <code>xml</code> parameter. Specifying both will cause an error.
layout: schema
name: IdpMetadata
properties_list:
- description: ''
  name: url
  type: object
- description: ''
  name: xml
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-idp-metadata-schema.json
slug: amazon-managed-grafana-idp-metadata
source_filename: amazon-managed-grafana-idp-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-idp-metadata-schema.json\",\n  \"title\": \"IdpMetadata\",\n  \"description\": \"A structure containing the identity provider (IdP) metadata used to integrate the identity provider with this workspace. You can specify the metadata either by providing a URL to its location in the <code>url</code> parameter, or by specifying the full metadata in XML format in the <code>xml</code> parameter. Specifying both will cause an error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdpMetadataUrl\"\n        },\n        {\n          \"description\": \"The URL of the location containing the IdP metadata.\"\n        }\n      ]\n    },\n    \"xml\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The full IdP metadata, in XML format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-idp-metadata-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: IdpMetadata
---
