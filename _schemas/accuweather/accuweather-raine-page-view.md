---
description: RainePageView schema from AccuWeather API
layout: schema
name: RainePageView
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: test
  type: string
- description: ''
  name: platform
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: page
  type: object
- description: ''
  name: ads
  type: object
- description: ''
  name: session
  type: object
- description: ''
  name: user
  type: object
- description: ''
  name: network
  type: object
- description: ''
  name: device
  type: object
- description: ''
  name: weather
  type: object
- description: True if X-Akamai-Bot header is filled; default false
  name: bot
  type: boolean
- description: ''
  name: time
  type: string
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-raine-page-view-schema.json
slug: accuweather-raine-page-view
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-raine-page-view-schema.json\",\n  \"title\": \"RainePageView\",\n  \"description\": \"RainePageView schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"test\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"page\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"group\": {\n          \"type\": \"string\",\n          \"description\": \"Page group like 'three-day' or 'hourly' designating the page category\",\n          \"nullable\": true\n        },\n        \"url\": {\n          \"\
  type\": \"string\",\n          \"description\": \"URL of the page\",\n          \"nullable\": true\n        },\n        \"referrer\": {\n          \"type\": \"string\",\n          \"description\": \"Referrer of the page\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"ads\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Simplified ad code for ad slots on the page.\\r\\nEg. '6581/web/us/*/news_info/country_home'\",\n          \"nullable\": true\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"One of 'active', 'missing', or 'restricted' indicating a user's ID status\\r\\nDefault missing.\",\n          \"nullable\": true\n        },\n        \"cookie3p\": {\n          \"type\": \"string\",\n          \"description\": \"One of 'active', 'missing', or 'restricted' indicating a user can access\
  \ 3rd party cookies or not.\\r\\nDefault missing.\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"session\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique ID for the user's session (persistent to 10m after the last pageview)\",\n          \"nullable\": true\n        },\n        \"partner\": {\n          \"type\": \"string\",\n          \"description\": \"Unique ID for the partner from the URL\",\n          \"nullable\": true\n        },\n        \"utm\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"source\": {\n              \"type\": \"string\",\n              \"description\": \"utm_source from the URL\",\n              \"nullable\": true\n            },\n            \"medium\": {\n              \"type\": \"string\",\n              \"description\": \"utm_medium from the URL\",\n              \"\
  nullable\": true\n            },\n            \"campaign\": {\n              \"type\": \"string\",\n              \"description\": \"utm_campaign from the URL\",\n              \"nullable\": true\n            },\n            \"term\": {\n              \"type\": \"string\",\n              \"description\": \"utm_term from the URL\",\n              \"nullable\": true\n            }\n          },\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"user\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique ID for the user (persistent across sessions)\",\n          \"nullable\": true\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"Language code set for the product for the user (en-us, en-gb, etc.)\",\n          \"nullable\": true\n        },\n        \"country\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Country code for the user's location.\\r\\nEg. US\",\n          \"nullable\": true\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"Region code for the user's location.\\r\\nEg. PA\",\n          \"nullable\": true\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City for the location\",\n          \"nullable\": true\n        },\n        \"dma\": {\n          \"type\": \"string\",\n          \"description\": \"DMA for the user's location.\\r\\nEg. 566. Not available outside of the US.\",\n          \"nullable\": true\n        },\n        \"start\": {\n          \"type\": \"string\",\n          \"description\": \"Date of the user's first visit.\\r\\nI.e. Cookie creation date\",\n          \"nullable\": true\n        },\n        \"offset\": {\n          \"type\": \"string\",\n          \"description\": \"Valid string of the user's current UTC offset in\
  \ hh:mm:ss format.\\r\\nEx. -05:00 or 05:00\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"network\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"throughput\": {\n          \"type\": \"string\",\n          \"description\": \"Category of 'network speed' for the user. Eg. 'vhigh'\",\n          \"nullable\": true\n        },\n        \"network\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the network for the user. Eg. 'comcast'\",\n          \"nullable\": true\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of network for the user. Eg. 'cable'\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"device\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the user's browser.\\\
  r\\nEg. 'Chrome'\",\n          \"nullable\": true\n        },\n        \"brand\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the user's device maker.\\r\\nEg. 'Apple' or 'Samsung'\",\n          \"nullable\": true\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Version of the user's browser.\\r\\nEg. '16'\",\n          \"nullable\": true\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"One of 'mobile', 'tablet', or 'desktop'\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"weather\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"Surefind location key for the user's weather location\\r\\nEg. 335315\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"bot\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"True if X-Akamai-Bot header is filled; default false\",\n      \"nullable\": true\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-raine-page-view-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: RainePageView
---
