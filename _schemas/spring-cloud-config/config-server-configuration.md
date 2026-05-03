---
description: JSON Schema for Spring Cloud Config Server application properties.
layout: schema
name: Spring Cloud Config Server Configuration
properties_list:
- description: ''
  name: spring
  type: object
provider_name: Spring Cloud Config
provider_slug: spring-cloud-config
schema_file: json-schema/config-server-configuration.json
slug: config-server-configuration
source_filename: config-server-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spring-cloud-config/json-schema/config-server-configuration.json\",\n  \"title\": \"Spring Cloud Config Server Configuration\",\n  \"description\": \"JSON Schema for Spring Cloud Config Server application properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spring\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cloud\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"config\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"server\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"git\": {\n                      \"$ref\": \"#/$defs/GitRepositoryConfig\"\n                    },\n                    \"native\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n\
  \                        \"searchLocations\": {\n                          \"type\": \"array\",\n                          \"items\": { \"type\": \"string\" },\n                          \"description\": \"Search locations for native profile.\"\n                        }\n                      }\n                    },\n                    \"vault\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"host\": { \"type\": \"string\" },\n                        \"port\": { \"type\": \"integer\", \"default\": 8200 },\n                        \"scheme\": { \"type\": \"string\", \"default\": \"https\" },\n                        \"backend\": { \"type\": \"string\", \"default\": \"secret\" },\n                        \"profileSeparator\": { \"type\": \"string\", \"default\": \",\" }\n                      }\n                    },\n                    \"defaultLabel\": {\n                      \"type\": \"string\",\n            \
  \          \"description\": \"Default label to use when none specified.\"\n                    },\n                    \"defaultProfile\": {\n                      \"type\": \"string\",\n                      \"default\": \"default\",\n                      \"description\": \"Default profile to use.\"\n                    },\n                    \"encrypt\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"enabled\": {\n                          \"type\": \"boolean\",\n                          \"default\": true,\n                          \"description\": \"Enable decryption of properties.\"\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"GitRepositoryConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uri\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"URI of the Git repository.\"\n        },\n        \"defaultLabel\": {\n          \"type\": \"string\",\n          \"description\": \"Default branch or tag.\"\n        },\n        \"searchPaths\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Search paths within the repository.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Git username for authentication.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Git password for authentication.\"\n        },\n        \"cloneOnStart\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to clone repository on startup.\"\n        },\n        \"timeout\": {\n          \"type\": \"integer\",\n          \"default\": 5,\n          \"description\": \"Timeout in seconds for obtaining HTTP/SSH\
  \ connection.\"\n        },\n        \"refreshRate\": {\n          \"type\": \"integer\",\n          \"default\": 0,\n          \"description\": \"Rate in seconds for refreshing the Git repository (0 = every request).\"\n        },\n        \"skipSslValidation\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to skip SSL certificate validation.\"\n        },\n        \"repos\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/GitRepositoryConfig\"\n          },\n          \"description\": \"Pattern-matched repository configurations.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spring-cloud-config/refs/heads/main/json-schema/config-server-configuration.json
tags:
- Configuration Management
- Distributed Systems
- Externalized Configuration
- Java
- Microservices
- Spring
- Spring Cloud
title: Spring Cloud Config Server Configuration
---
