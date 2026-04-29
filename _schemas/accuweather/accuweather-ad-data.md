---
description: AdData schema from AccuWeather API
layout: schema
name: AdData
properties_list:
- description: ''
  name: globalAdConfig
  type: object
- description: ''
  name: ortbConfig
  type: object
- description: ''
  name: adPageInfo
  type: object
- description: ''
  name: adSlots
  type: object
- description: ''
  name: adInfo
  type: object
- description: ''
  name: uspString
  type: string
- description: ''
  name: ppid
  type: string
- description: ''
  name: isPrebidDisabled
  type: boolean
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-ad-data-schema.json
slug: accuweather-ad-data
source_filename: accuweather-ad-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ad-data-schema.json\",\n  \"title\": \"AdData\",\n  \"description\": \"AdData schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"globalAdConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prebidTimeout\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        },\n        \"awxTimeout\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        },\n        \"bundleUrl\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"deprecated\": true\n        },\n        \"bundleId\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"gptEnableSingleRequest\": {\n          \"type\": \"boolean\"\n        },\n        \"gptLazyLoading\": {\n   \
  \       \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"buyItNowSkipGoogleAdManager\": {\n          \"type\": \"boolean\"\n        },\n        \"testVariant\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"deviceClass\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"disableInitialAdLoad\": {\n          \"type\": \"boolean\"\n        },\n        \"javascriptHead\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"javascriptBody\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"ortbConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"domain\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"\
  categories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"nullable\": true\n        },\n        \"sectionCategories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"nullable\": true\n        },\n        \"pageCategories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"nullable\": true\n        },\n        \"keywords\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"pageUrl\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"referrerUrl\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"isOptimizedForMobile\": {\n          \"type\": \"boolean\"\n        },\n        \"hasPrivacyPolicy\": {\n          \"type\": \"boolean\"\n        },\n        \"publisher\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"domain\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"categories\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"nullable\": true\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"content\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"title\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"categories\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\
  \n              },\n              \"nullable\": true\n            },\n            \"productQuality\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"context\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"keywords\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"sourceRelationship\": {\n              \"enum\": [\n                \"Indirect\",\n                \"Direct\"\n              ],\n              \"type\": \"string\"\n            },\n            \"language\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"nullable\": true\n                },\n                \"extensions\": {\n       \
  \           \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"nullable\": true\n                  },\n                  \"nullable\": true\n                },\n                \"segments\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"name\": {\n                        \"type\": \"string\",\n                        \"nullable\": true\n                      },\n                      \"value\": {\n                        \"type\": \"string\",\n                        \"nullable\": true\n                      }\n                    },\n                    \"additionalProperties\": false\n                  },\n                  \"nullable\": true\n                }\n              },\n              \"additionalProperties\": false\n            }\n          },\n          \"additionalProperties\": false\n        }\n  \
  \    },\n      \"additionalProperties\": false\n    },\n    \"adPageInfo\": {\n      \"type\": \"object\",\n      \"additionalProperties\": false\n    },\n    \"adSlots\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/Ad\"\n      },\n      \"nullable\": true\n    },\n    \"adInfo\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    },\n    \"uspString\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"ppid\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isPrebidDisabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-ad-data-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: AdData
---
