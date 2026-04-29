---
description: ''
layout: schema
name: GetListViewRecordsperAPIName
properties_list:
- description: ''
  name: count
  type: integer
- description: ''
  name: currentPageToken
  type: string
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: fields
  type: array
- description: ''
  name: listInfoETag
  type: string
- description: ''
  name: listReference
  type: object
- description: ''
  name: nextPageToken
  type: string
- description: ''
  name: nextPageUrl
  type: string
- description: ''
  name: optionalFields
  type: array
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: previousPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: previousPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: records
  type: array
- description: ''
  name: searchTerm
  type: '[''string'', ''null'']'
- description: ''
  name: sortBy
  type: string
- description: ''
  name: where
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-list-view-recordsper-api-name-schema.json
slug: salesforce-get-list-view-recordsper-api-name
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"currentPageToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"listInfoETag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"listReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"listViewApiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"objectApiName\": {\n          \"type\": \"string\",\n          \"example\"\
  : \"example_value\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"listViewApiName\",\n        \"objectApiName\",\n        \"type\"\n      ]\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"nextPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"optionalFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"previousPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"previousPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"records\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"apiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"childRelationships\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"eTag\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fields\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"BillingCountry\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"['string', 'null']\",\n                \
  \    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"CreatedDate\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"Id\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n            \
  \        \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"LastModifiedById\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"LastModifiedDate\": {\n        \
  \        \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"Name\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\"\
  : [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"Owner\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"apiName\": {\n                        \"type\": \"object\"\n                      },\n                      \"childRelationships\": {\n                        \"type\": \"object\"\n                      },\n                      \"eTag\": {\n                        \"type\": \"object\"\n                      },\n                      \"fields\": {\n                        \"type\": \"object\"\n                      },\n                      \"id\": {\n                        \"type\": \"object\"\
  \n                      },\n                      \"lastModifiedById\": {\n                        \"type\": \"object\"\n                      },\n                      \"lastModifiedDate\": {\n                        \"type\": \"object\"\n                      },\n                      \"recordTypeId\": {\n                        \"type\": \"object\"\n                      },\n                      \"recordTypeInfo\": {\n                        \"type\": \"object\"\n                      },\n                      \"systemModstamp\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"apiName\",\n                      \"childRelationships\",\n                      \"eTag\",\n                      \"fields\",\n                      \"id\",\n                      \"lastModifiedById\",\n                      \"lastModifiedDate\"\n                    ]\n                  }\n         \
  \       },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"OwnerId\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"Phone\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n     \
  \             \"value\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"Site\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"SystemModstamp\": {\n                \"type\": \"object\",\n                \"properties\"\
  : {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n                  \"value\"\n                ]\n              },\n              \"Type\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"displayValue\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  },\n                  \"value\": {\n                    \"type\": \"['string', 'null']\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"displayValue\",\n   \
  \               \"value\"\n                ]\n              }\n            },\n            \"required\": [\n              \"BillingCountry\",\n              \"CreatedDate\",\n              \"Id\",\n              \"LastModifiedById\",\n              \"LastModifiedDate\",\n              \"Name\",\n              \"Owner\",\n              \"OwnerId\",\n              \"Phone\",\n              \"Site\",\n              \"SystemModstamp\",\n              \"Type\"\n            ]\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"lastModifiedById\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"lastModifiedDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"recordTypeId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"recordTypeInfo\": {\n   \
  \         \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"systemModstamp\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"apiName\",\n          \"childRelationships\",\n          \"eTag\",\n          \"fields\",\n          \"id\",\n          \"lastModifiedById\",\n          \"lastModifiedDate\",\n          \"recordTypeId\",\n          \"recordTypeInfo\",\n          \"systemModstamp\"\n        ]\n      }\n    },\n    \"searchTerm\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"sortBy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"where\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"count\",\n    \"currentPageToken\",\n    \"currentPageUrl\",\n    \"fields\",\n    \"listInfoETag\"\
  ,\n    \"listReference\",\n    \"nextPageToken\",\n    \"nextPageUrl\",\n    \"optionalFields\",\n    \"pageSize\",\n    \"previousPageToken\",\n    \"previousPageUrl\",\n    \"records\",\n    \"searchTerm\",\n    \"sortBy\",\n    \"where\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetListViewRecordsperAPIName\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-list-view-recordsper-api-name-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: GetListViewRecordsperAPIName
---
