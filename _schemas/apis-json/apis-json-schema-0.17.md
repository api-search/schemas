---
description: ''
layout: schema
name: A JSON Schema for apis.json, version 0.17
properties_list:
- description: The type of the APIs.json collection.
  name: type
  type: string
- description: The name of the service described
  name: name
  type: string
- description: Description of the service
  name: description
  type: string
- description: URL where the apis.json file will live
  name: url
  type: string
- description: Image to represent the API
  name: image
  type: string
- description: Date when the file was created
  name: created
  type: string
- description: Date when the file was modified
  name: modified
  type: string
- description: APIs.json spec version, latest is 0.17
  name: specificationVersion
  type: string
- description: All the APIs of this service
  name: apis
  type: array
- description: Maintainers of the apis.json file
  name: maintainers
  type: array
- description: Tags to describe the service
  name: tags
  type: array
- description: Links to other apis.json definitions included in this service
  name: include
  type: array
- description: Common properties that apply across all APIs.
  name: common
  type: array
- description: Links to other apis.json that will be overlaid original.
  name: overlays
  type: array
provider_name: APIs.json
provider_slug: apis-json
schema_file: json-schema/apis-json-schema-0.17.json
slug: apis-json-schema-0.17
source_json: "{\n  \"title\": \"A JSON Schema for apis.json, version 0.17\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": false,\n  \"patternProperties\": {\n    \"^X-\": {\n      \"type\": \"object\"\n    }\n  },\n  \"$defs\": {\n    \"maintainers\": {\n      \"description\": \"The person or organization responsible for maintaining the API\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"name\",\n          \"minLength\": 5\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"apis\": {\n      \"description\": \"The description of the API\",\n      \"required\": [\n        \"name\",\n        \"description\",\n        \"image\",\n        \"baseURL\",\n        \"humanURL\",\n        \"properties\"\n      ],\n      \"properties\": {\n        \"aid\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"unique identifier for API\",\n          \"minLength\": 10\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"name\",\n          \"minLength\": 5\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"description of the API\",\n          \"minLength\": 5\n        },\n        \"image\": {\n          \"type\": \"string\",\n          \"description\": \"URL of an image representing the API\"\n        },\n        \"baseURL\": {\n          \"type\": \"string\",\n          \"pattern\": \"^(http)|(https)://(.*)$\",\n          \"description\": \"baseURL\"\n        },\n        \"humanURL\": {\n          \"type\": \"string\",\n          \"pattern\": \"^(http)|(https)://(.*)$\",\n          \"description\": \"humanURL\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n\
  \            \"minLength\": 1\n          },\n          \"description\": \"tags to describe the API\"\n        },\n        \"properties\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/urls\"\n          },\n          \"description\": \"URLs\"\n        },\n        \"contact\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/contact\"\n          },\n          \"description\": \"Contact to reach if questions about API\"\n        },\n        \"meta\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/metaInformation\"\n          }\n        }\n      }\n    },\n    \"metaInformation\": {\n      \"description\": \"Metadata about the API\",\n      \"required\": [\n        \"key\",\n        \"value\"\n      ],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\"\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n     \
  \ }\n    },\n    \"contact\": {\n      \"description\": \"Information on contacting the API support\",\n      \"required\": [\n        \"FN\"\n      ],\n      \"additionalProperties\": true,\n      \"patternProperties\": {\n        \"^X-\": {\n          \"type\": \"string\"\n        }\n      },\n      \"properties\": {\n        \"FN\": {\n          \"type\": \"string\",\n          \"minLength\": 1\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\",\n          \"minLength\": 1\n        },\n        \"adr\": {\n          \"type\": \"string\"\n        },\n        \"tel\": {\n          \"type\": \"string\",\n          \"minLength\": 1\n        },\n        \"X-twitter\": {\n          \"type\": \"string\"\n        },\n        \"X-github\": {\n          \"type\": \"string\"\n        },\n        \"photo\": {\n          \"type\": \"string\",\n          \"pattern\": \"^(http)|(https)://(.*)$\"\
  \n        },\n        \"vCard\": {\n          \"type\": \"string\",\n          \"pattern\": \"^(http)|(https)://(.*)$\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"pattern\": \"^(http)|(https)://(.*)$\"\n        }\n      }\n    },\n    \"urls\": {\n      \"description\": \"A representation of a URL\",\n      \"required\": [\n        \"type\",\n        \"url\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the property.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"One of the designated API property types or a custom one prefixed with x-.\",\n          \"pattern\": \"^(Swagger)$|^(OpenAPI)$|^(JSONSchema)$|^(GraphQLSchema)$|^(PostmanCollection)$|^(PostmanWorkspace)$|^(AsyncAPI)$|^(RAML)$|^(Blueprint)$|^(WADL)$|^(WSDL)$|^(GettingStarted)$|^(Documentation)$|^(Authentication)$|^(Versioning)$|^(Signup)$|^(Login)$|^(TermsOfService)$|^(InterfaceLicense)$|^(PrivacyPolicy)$|^(DeprecationPolicy)$|^(ServiceLevelAgreement)$|^(Security)$|^(SDKs)$|^(StatusPage)$|^(Pricing)$|^(RateLimits)$|^(Blog)$|^(BlogFeed)$|^(Forums)$|^(Support)$|^(ChangeLog)$|^(RoadMap)$|^(Contact)$|^(ErrorCodes)$|^(GitHubOrg)$|^(GitHubRepo)$|^(Twitter)$|^(AlertsTwitterHandle)$|^(Webhooks)$|^(Integrations)$|^(OpenAIPluginManifest)$|^(X-[A-Za-z0-9\\\
  \\-]*)$\"\n        },\n        \"mediaType\": {\n          \"type\": \"string\",\n          \"description\": \"IANA media type representing the property.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"The URL for the property. * must be url or data.\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"description\": \"The data for the property. * must be url or data\"\n        }\n      }\n    },\n    \"tags\": {\n      \"description\": \"A consistent set of tag to apply to a description\"\n    },\n    \"include\": {\n      \"description\": \"Include other APIs.json file\",\n      \"required\": [\n        \"name\",\n        \"url\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"minLength\": 1\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"overlay\": {\n      \"description\": \"Overlay other APIs.json file\"\
  ,\n      \"required\": [\n        \"url\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"minLength\": 1\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"description\",\n    \"url\",\n    \"apis\",\n    \"maintainers\",\n    \"tags\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the APIs.json collection.\",\n      \"enum\": [\n        \"Index\",\n        \"Template\",\n        \"Example\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service described\",\n      \"minLength\": 3,\n      \"maxLength\": 50\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service\",\n      \"minLength\": 5,\n      \"maxLength\": 1000\n    },\n    \"url\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"URL where the apis.json file will live\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Image to represent the API\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the file was created\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the file was modified\"\n    },\n    \"specificationVersion\": {\n      \"type\": \"string\",\n      \"description\": \"APIs.json spec version, latest is 0.17\"\n    },\n    \"apis\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/apis\"\n      },\n      \"description\": \"All the APIs of this service\"\n    },\n    \"maintainers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/contact\"\n      },\n      \"description\": \"Maintainers of\
  \ the apis.json file\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/tags\"\n      },\n      \"description\": \"Tags to describe the service\"\n    },\n    \"include\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/include\"\n      },\n      \"description\": \"Links to other apis.json definitions included in this service\"\n    },\n    \"common\": {\n      \"description\": \"Common properties that apply across all APIs.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/urls\"\n      }\n    },\n    \"overlays\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/overlay\"\n      },\n      \"description\": \"Links to other apis.json that will be overlaid original.\"\n    }\n  },\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/json-schema/apis-json-schema-0.17.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/json-schema/apis-json-schema-0.17.json
tags:
- API Aggregation
- API Cataloging
- API Commons
- API Discovery
- API Governance
- API Operations
- Machine Readable
- Specification
- Standard
title: A JSON Schema for apis.json, version 0.17
---
