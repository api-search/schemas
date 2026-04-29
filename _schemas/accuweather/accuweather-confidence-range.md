---
description: ConfidenceRange schema from AccuWeather API
layout: schema
name: ConfidenceRange
properties_list:
- description: ''
  name: lower
  type: object
- description: ''
  name: low
  type: object
- description: ''
  name: likely
  type: object
- description: ''
  name: high
  type: object
- description: ''
  name: higher
  type: object
provider_name: AccuWeather
provider_slug: accuweather
schema_file: json-schema/accuweather-confidence-range-schema.json
slug: accuweather-confidence-range
source_filename: accuweather-confidence-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-confidence-range-schema.json\",\n  \"title\": \"ConfidenceRange\",\n  \"description\": \"ConfidenceRange schema from AccuWeather API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lower\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayAmount\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"low\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\
  \n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"high\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"probability\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"low\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayAmount\"\
  : {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"low\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"high\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n           \
  \   \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"probability\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"likely\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayAmount\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"low\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n      \
  \        \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"high\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"probability\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"high\": {\n  \
  \    \"type\": \"object\",\n      \"properties\": {\n        \"displayAmount\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"low\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"high\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n            \
  \  \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"probability\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"higher\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayAmount\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        },\n        \"low\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n       \
  \       \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"high\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"nullable\": true\n            },\n            \"unit\": {\n              \"type\": \"string\",\n              \"nullable\": true\n            },\n            \"unitType\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"probability\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"nullable\": true\n        },\n        \"phrase\": {\n          \"type\": \"string\",\n          \"nullable\": true\n        }\n\
  \      },\n      \"additionalProperties\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accuweather/refs/heads/main/json-schema/accuweather-confidence-range-schema.json
tags:
- Weather
- Forecasts
- Meteorology
- Location Services
- Air Quality
- Storms
title: ConfidenceRange
---
