---
description: UpdateDevEndpointRequest schema from Amazon Glue API
layout: schema
name: UpdateDevEndpointRequest
properties_list:
- description: ''
  name: EndpointName
  type: object
- description: ''
  name: PublicKey
  type: object
- description: ''
  name: AddPublicKeys
  type: object
- description: ''
  name: DeletePublicKeys
  type: object
- description: ''
  name: CustomLibraries
  type: object
- description: ''
  name: UpdateEtlLibraries
  type: object
- description: ''
  name: DeleteArguments
  type: object
- description: ''
  name: AddArguments
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-dev-endpoint-request-schema.json
slug: glue-update-dev-endpoint-request
source_filename: glue-update-dev-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-dev-endpoint-request-schema.json\",\n  \"title\": \"UpdateDevEndpointRequest\",\n  \"description\": \"UpdateDevEndpointRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the <code>DevEndpoint</code> to be updated.\"\n        }\n      ]\n    },\n    \"PublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The public key for the <code>DevEndpoint</code> to use.\"\n        }\n      ]\n    },\n    \"AddPublicKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublicKeysList\"\
  \n        },\n        {\n          \"description\": \"The list of public keys for the <code>DevEndpoint</code> to use.\"\n        }\n      ]\n    },\n    \"DeletePublicKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublicKeysList\"\n        },\n        {\n          \"description\": \"The list of public keys to be deleted from the <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"CustomLibraries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpointCustomLibraries\"\n        },\n        {\n          \"description\": \"Custom Python or Java libraries to be loaded in the <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"UpdateEtlLibraries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanValue\"\n        },\n        {\n          \"description\": \" <code>True</code> if the list of custom libraries to be loaded in the development endpoint needs to be updated,\
  \ or <code>False</code> if otherwise.\"\n        }\n      ]\n    },\n    \"DeleteArguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The list of argument keys to be deleted from the map of arguments used to configure the <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"AddArguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapValue\"\n        },\n        {\n          \"description\": \"<p>The map of arguments to add the map of arguments used to configure the <code>DevEndpoint</code>.</p> <p>Valid arguments are:</p> <ul> <li> <p> <code>\\\"--enable-glue-datacatalog\\\": \\\"\\\"</code> </p> </li> </ul> <p>You can specify a version of Python support for development endpoints by using the <code>Arguments</code> parameter in the <code>CreateDevEndpoint</code> or <code>UpdateDevEndpoint</code> APIs. If no arguments are provided, the version\
  \ defaults to Python 2.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-dev-endpoint-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateDevEndpointRequest
---
