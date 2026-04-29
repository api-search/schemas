---
description: OrtbSite schema from AccuWeather API
layout: schema
name: OrtbSite
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: domain
  type: string
- description: ''
  name: categories
  type: array
- description: ''
  name: sectionCategories
  type: array
- description: ''
  name: pageCategories
  type: array
- description: ''
  name: keywords
  type: string
- description: ''
  name: pageUrl
  type: string
- description: ''
  name: referrerUrl
  type: string
- description: ''
  name: isOptimizedForMobile
  type: boolean
- description: ''
  name: hasPrivacyPolicy
  type: boolean
- description: ''
  name: publisher
  type: object
- description: ''
  name: content
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ortb-site-schema.json
slug: accuweather-ortb-site
source_filename: accuweather-ortb-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-site-schema.json\",\n  \"title\": \"OrtbSite\",\n  \"description\": \"OrtbSite schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    },\n    \"sectionCategories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    },\n    \"pageCategories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    },\n    \"keywords\": {\n      \"type\"\
  : \"string\",\n      \"nullable\": true\n    },\n    \"pageUrl\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"referrerUrl\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isOptimizedForMobile\": {\n      \"type\": \"boolean\"\n    },\n    \"hasPrivacyPolicy\": {\n      \"type\": \"boolean\"\n    },\n    \"publisher\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"domain\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"nullable\"\
  : true\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"nullable\": true\n        },\n        \"productQuality\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"context\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"keywords\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"sourceRelationship\": {\n          \"enum\": [\n            \"Indirect\",\n            \"Direct\"\n          ],\n          \"type\": \"string\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\
  ,\n              \"nullable\": true\n            },\n            \"extensions\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"nullable\": true\n              },\n              \"nullable\": true\n            },\n            \"segments\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"nullable\": true\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"nullable\": true\n                  }\n                },\n                \"additionalProperties\": false\n              },\n              \"nullable\": true\n            }\n          },\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\"\
  : false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ortb-site-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: OrtbSite
---
