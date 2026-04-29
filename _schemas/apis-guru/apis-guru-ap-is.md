---
description: List of API details. It is a JSON object with API IDs(`<provider>[:<service>]`) as keys.
layout: schema
name: APIs
properties_list: []
provider_name: APIs.guru
provider_slug: apis-guru
schema_file: json-schema/apis-guru-ap-is-schema.json
slug: apis-guru-ap-is
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-ap-is-schema.json\",\n  \"title\": \"APIs\",\n  \"description\": \"List of API details.\\nIt is a JSON object with API IDs(`<provider>[:<service>]`) as keys.\\n\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/API\"\n  },\n  \"example\": {\n    \"googleapis.com:drive\": {\n      \"added\": \"2015-02-22 20:00:45+00:00\",\n      \"preferred\": \"v3\",\n      \"versions\": {\n        \"v2\": {\n          \"added\": \"2015-02-22 20:00:45+00:00\",\n          \"info\": {\n            \"title\": \"Drive\",\n            \"version\": \"v2\",\n            \"x-apiClientRegistration\": {\n              \"url\": \"https://console.developers.google.com\"\n            },\n            \"x-logo\": {\n              \"url\": \"https://api.apis.guru/v2/cache/logo/https_www.gstatic.com_images_icons_material_product_2x_drive_32dp.png\"\
  \n            },\n            \"x-origin\": {\n              \"format\": \"google\",\n              \"url\": \"https://www.googleapis.com/discovery/v1/apis/drive/v2/rest\",\n              \"version\": \"v1\"\n            },\n            \"x-preferred\": false,\n            \"x-providerName\": \"googleapis.com\",\n            \"x-serviceName\": \"drive\"\n          },\n          \"swaggerUrl\": \"https://api.apis.guru/v2/specs/googleapis.com/drive/v2/swagger.json\",\n          \"swaggerYamlUrl\": \"https://api.apis.guru/v2/specs/googleapis.com/drive/v2/swagger.yaml\",\n          \"updated\": \"2016-06-17 00:21:44+00:00\"\n        },\n        \"v3\": {\n          \"added\": \"2015-12-12 00:25:13+00:00\",\n          \"info\": {\n            \"title\": \"Drive\",\n            \"version\": \"v3\",\n            \"x-apiClientRegistration\": {\n              \"url\": \"https://console.developers.google.com\"\n            },\n            \"x-logo\": {\n              \"url\": \"https://api.apis.guru/v2/cache/logo/https_www.gstatic.com_images_icons_material_product_2x_drive_32dp.png\"\
  \n            },\n            \"x-origin\": {\n              \"format\": \"google\",\n              \"url\": \"https://www.googleapis.com/discovery/v1/apis/drive/v3/rest\",\n              \"version\": \"v1\"\n            },\n            \"x-preferred\": true,\n            \"x-providerName\": \"googleapis.com\",\n            \"x-serviceName\": \"drive\"\n          },\n          \"swaggerUrl\": \"https://api.apis.guru/v2/specs/googleapis.com/drive/v3/swagger.json\",\n          \"swaggerYamlUrl\": \"https://api.apis.guru/v2/specs/googleapis.com/drive/v3/swagger.yaml\",\n          \"updated\": \"2016-06-17 00:21:44+00:00\"\n        }\n      }\n    }\n  },\n  \"minProperties\": 1,\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-ap-is-schema.json
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
title: APIs
---
