---
description: Paginated list of catalogs
layout: schema
name: CatalogListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Pagination links following JSON:API conventions
  name: links
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-catalog-list-response-schema.json
slug: prime-api-catalog-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-catalog-list-response-schema.json\",\n  \"title\": \"CatalogListResponse\",\n  \"description\": \"Paginated list of catalogs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A catalog that organizes and controls access to learning objects\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique catalog identifier\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"const\": \"catalog\"\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"dateCreated\": {\n                \"type\": \"string\",\n  \
  \              \"format\": \"date-time\",\n                \"description\": \"Timestamp when the catalog was created\"\n              },\n              \"dateUpdated\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Timestamp of the last update\"\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"Catalog description\"\n              },\n              \"isDefault\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether this is the default catalog\"\n              },\n              \"isInternallySearchable\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether learning objects in this catalog appear in search\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Catalog name\"\n              },\n            \
  \  \"state\": {\n                \"type\": \"string\",\n                \"description\": \"Catalog state\",\n                \"enum\": [\n                  \"Enabled\",\n                  \"Disabled\"\n                ]\n              }\n            }\n          },\n          \"relationships\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"learningObjects\": {\n                \"type\": \"object\",\n                \"description\": \"A JSON:API relationship object\",\n                \"properties\": {\n                  \"data\": {\n                    \"oneOf\": [\n                      {\n                        \"type\": \"object\",\n                        \"description\": \"JSON:API resource identifier\",\n                        \"required\": [\n                          \"id\",\n                          \"type\"\n                        ],\n                        \"properties\": {\n                          \"id\": {\n                   \
  \         \"type\": \"string\",\n                            \"description\": \"Resource identifier\"\n                          },\n                          \"type\": {\n                            \"type\": \"string\",\n                            \"description\": \"Resource type name\"\n                          }\n                        }\n                      },\n                      {\n                        \"type\": \"array\",\n                        \"items\": {\n                          \"type\": \"object\",\n                          \"description\": \"JSON:API resource identifier\",\n                          \"required\": [\n                            \"id\",\n                            \"type\"\n                          ],\n                          \"properties\": {\n                            \"id\": {\n                              \"type\": \"string\",\n                              \"description\": \"Resource identifier\"\n                            },\n\
  \                            \"type\": {\n                              \"type\": \"string\",\n                              \"description\": \"Resource type name\"\n                            }\n                          }\n                        }\n                      }\n                    ]\n                  },\n                  \"links\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"related\": {\n                        \"type\": \"string\",\n                        \"format\": \"uri\",\n                        \"description\": \"URL to fetch the related resource\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination links following JSON:API conventions\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"\
  string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the current page\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page\"\n        },\n        \"prev\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the previous page\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-catalog-list-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: CatalogListResponse
---
