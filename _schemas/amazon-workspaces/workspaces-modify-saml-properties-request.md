---
description: ModifySamlPropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifySamlPropertiesRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: SamlProperties
  type: object
- description: ''
  name: PropertiesToDelete
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-saml-properties-request-schema.json
slug: workspaces-modify-saml-properties-request
source_filename: workspaces-modify-saml-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\"\n  ],\n  \"title\": \"ModifySamlPropertiesRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier for which you want to configure SAML properties.\"\n        }\n      ]\n    },\n    \"SamlProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlProperties\"\n        },\n        {\n          \"description\": \"The properties for configuring SAML 2.0 authentication.\"\n        }\n      ]\n    },\n    \"PropertiesToDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeletableSamlPropertiesList\"\n        },\n        {\n          \"description\": \"<p>The SAML properties to delete as part of your request.</p> <p>Specify one of the following options:</p> <ul> <li> <p> <code>SAML_PROPERTIES_USER_ACCESS_URL</code>\
  \ to delete the user access URL.</p> </li> <li> <p> <code>SAML_PROPERTIES_RELAY_STATE_PARAMETER_NAME</code> to delete the relay state parameter name.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-saml-properties-request-schema.json\",\n  \"description\": \"ModifySamlPropertiesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-saml-properties-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifySamlPropertiesRequest
---
