---
description: A structure that defines which attributes in the IdP assertion are to be used to define information about the users authenticated by the IdP to use the workspace.
layout: schema
name: AssertionAttributes
properties_list:
- description: ''
  name: email
  type: object
- description: ''
  name: groups
  type: object
- description: ''
  name: login
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: org
  type: object
- description: ''
  name: role
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-assertion-attributes-schema.json
slug: amazon-managed-grafana-assertion-attributes
source_filename: amazon-managed-grafana-assertion-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-assertion-attributes-schema.json\",\n  \"title\": \"AssertionAttributes\",\n  \"description\": \"A structure that defines which attributes in the IdP assertion are to be used to define information about the users authenticated by the IdP to use the workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttribute\"\n        },\n        {\n          \"description\": \"The name of the attribute within the SAML assertion to use as the email names for SAML users.\"\n        }\n      ]\n    },\n    \"groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttribute\"\n        },\n        {\n          \"description\": \"The name of the\
  \ attribute within the SAML assertion to use as the user full \\\"friendly\\\" names for user groups.\"\n        }\n      ]\n    },\n    \"login\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttribute\"\n        },\n        {\n          \"description\": \"The name of the attribute within the SAML assertion to use as the login names for SAML users.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttribute\"\n        },\n        {\n          \"description\": \"The name of the attribute within the SAML assertion to use as the user full \\\"friendly\\\" names for SAML users.\"\n        }\n      ]\n    },\n    \"org\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttribute\"\n        },\n        {\n          \"description\": \"The name of the attribute within the SAML assertion to use as the user full \\\"friendly\\\" names for\
  \ the users' organizations.\"\n        }\n      ]\n    },\n    \"role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssertionAttribute\"\n        },\n        {\n          \"description\": \"The name of the attribute within the SAML assertion to use as the user roles.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-assertion-attributes-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: AssertionAttributes
---
