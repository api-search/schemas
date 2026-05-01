---
description: A structure containing information about how this workspace works with SAML.
layout: schema
name: SamlConfiguration
properties_list:
- description: ''
  name: allowedOrganizations
  type: object
- description: ''
  name: assertionAttributes
  type: object
- description: ''
  name: idpMetadata
  type: object
- description: ''
  name: loginValidityDuration
  type: object
- description: ''
  name: roleValues
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-saml-configuration-schema.json
slug: amazon-managed-grafana-saml-configuration
source_filename: amazon-managed-grafana-saml-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-saml-configuration-schema.json\",\n  \"title\": \"SamlConfiguration\",\n  \"description\": \"A structure containing information about how this workspace works with SAML. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedOrganizations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowedOrganizations\"\n        },\n        {\n          \"description\": \"Lists which organizations defined in the SAML assertion are allowed to use the Amazon Managed Grafana workspace. If this is empty, all organizations in the assertion attribute have access.\"\n        }\n      ]\n    },\n    \"assertionAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttributes\"\n        },\n        {\n      \
  \    \"description\": \"A structure that defines which attributes in the SAML assertion are to be used to define information about the users authenticated by that IdP to use the workspace.\"\n        }\n      ]\n    },\n    \"idpMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdpMetadata\"\n        },\n        {\n          \"description\": \"A structure containing the identity provider (IdP) metadata used to integrate the identity provider with this workspace.\"\n        }\n      ]\n    },\n    \"loginValidityDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginValidityDuration\"\n        },\n        {\n          \"description\": \"How long a sign-on session by a SAML user is valid, before the user has to sign on again.\"\n        }\n      ]\n    },\n    \"roleValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleValues\"\n        },\n        {\n          \"description\"\
  : \"A structure containing arrays that map group names in the SAML assertion to the Grafana <code>Admin</code> and <code>Editor</code> roles in the workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"idpMetadata\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-saml-configuration-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: SamlConfiguration
---
