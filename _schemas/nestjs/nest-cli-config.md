---
description: JSON Schema for the nest-cli.json configuration file used by the NestJS CLI for project management, compilation, and monorepo/workspace settings.
layout: schema
name: NestJS CLI Configuration (nest-cli.json)
properties_list:
- description: JSON Schema reference
  name: $schema
  type: string
- description: Schematics collection to use for generating components
  name: collection
  type: string
- description: Root directory for source files
  name: sourceRoot
  type: string
- description: Root directory of the project (monorepo)
  name: root
  type: string
- description: Entry file name (without extension)
  name: entryFile
  type: string
- description: Whether this is a monorepo workspace
  name: monorepo
  type: boolean
- description: Programming language
  name: language
  type: string
- description: Compiler settings for nest build
  name: compilerOptions
  type: object
- description: Default options for nest generate command
  name: generateOptions
  type: object
- description: Projects in a monorepo workspace
  name: projects
  type: object
provider_name: NestJS
provider_slug: nestjs
schema_file: json-schema/nest-cli-config.json
slug: nest-cli-config
source_filename: nest-cli-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/nestjs/json-schema/nest-cli-config.json\",\n  \"title\": \"NestJS CLI Configuration (nest-cli.json)\",\n  \"description\": \"JSON Schema for the nest-cli.json configuration file used by the NestJS CLI for project management, compilation, and monorepo/workspace settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"$schema\": {\n      \"type\": \"string\",\n      \"description\": \"JSON Schema reference\"\n    },\n    \"collection\": {\n      \"type\": \"string\",\n      \"default\": \"@nestjs/schematics\",\n      \"description\": \"Schematics collection to use for generating components\"\n    },\n    \"sourceRoot\": {\n      \"type\": \"string\",\n      \"default\": \"src\",\n      \"description\": \"Root directory for source files\"\n    },\n    \"root\": {\n      \"type\": \"string\",\n      \"default\": \"\",\n      \"description\": \"Root directory of\
  \ the project (monorepo)\"\n    },\n    \"entryFile\": {\n      \"type\": \"string\",\n      \"default\": \"main\",\n      \"description\": \"Entry file name (without extension)\"\n    },\n    \"monorepo\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether this is a monorepo workspace\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"enum\": [\"ts\", \"js\"],\n      \"default\": \"ts\",\n      \"description\": \"Programming language\"\n    },\n    \"compilerOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Compiler settings for nest build\",\n      \"properties\": {\n        \"tsConfigPath\": {\n          \"type\": \"string\",\n          \"default\": \"tsconfig.build.json\",\n          \"description\": \"Path to TypeScript configuration\"\n        },\n        \"webpack\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Use webpack for compilation\"\n        },\n\
  \        \"webpackConfigPath\": {\n          \"type\": \"string\",\n          \"default\": \"webpack.config.js\",\n          \"description\": \"Path to webpack configuration\"\n        },\n        \"plugins\": {\n          \"type\": \"array\",\n          \"description\": \"NestJS CLI plugins (e.g., @nestjs/swagger)\",\n          \"items\": {\n            \"oneOf\": [\n              {\n                \"type\": \"string\",\n                \"description\": \"Plugin package name\"\n              },\n              {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"description\": \"Plugin package name\"\n                  },\n                  \"options\": {\n                    \"type\": \"object\",\n                    \"description\": \"Plugin-specific options\",\n                    \"properties\": {\n                      \"dtoFileNameSuffix\": {\n                \
  \        \"type\": \"array\",\n                        \"items\": { \"type\": \"string\" },\n                        \"default\": [\".dto.ts\", \".entity.ts\"],\n                        \"description\": \"DTO file name suffixes for Swagger plugin\"\n                      },\n                      \"controllerFileNameSuffix\": {\n                        \"type\": \"string\",\n                        \"default\": \".controller.ts\"\n                      },\n                      \"classValidatorShim\": {\n                        \"type\": \"boolean\",\n                        \"default\": true\n                      },\n                      \"dtoKeyOfComment\": {\n                        \"type\": \"string\",\n                        \"default\": \"description\"\n                      },\n                      \"controllerKeyOfComment\": {\n                        \"type\": \"string\",\n                        \"default\": \"description\"\n                      },\n                   \
  \   \"introspectComments\": {\n                        \"type\": \"boolean\",\n                        \"default\": false\n                      }\n                    },\n                    \"additionalProperties\": true\n                  }\n                },\n                \"required\": [\"name\"]\n              }\n            ]\n          }\n        },\n        \"assets\": {\n          \"type\": \"array\",\n          \"description\": \"Non-TypeScript assets to distribute\",\n          \"items\": {\n            \"oneOf\": [\n              {\n                \"type\": \"string\",\n                \"description\": \"Glob pattern for assets\"\n              },\n              {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"include\": {\n                    \"type\": \"string\",\n                    \"description\": \"Glob pattern\"\n                  },\n                  \"exclude\": {\n                    \"type\": \"string\",\n   \
  \                 \"description\": \"Exclusion glob pattern\"\n                  },\n                  \"outDir\": {\n                    \"type\": \"string\",\n                    \"description\": \"Output directory\"\n                  },\n                  \"watchAssets\": {\n                    \"type\": \"boolean\",\n                    \"default\": false\n                  }\n                },\n                \"required\": [\"include\"]\n              }\n            ]\n          }\n        },\n        \"watchAssets\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Watch non-TS assets in watch mode\"\n        },\n        \"deleteOutDir\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Delete output directory before build\"\n        },\n        \"builder\": {\n          \"type\": \"string\",\n          \"enum\": [\"tsc\", \"webpack\", \"swc\"],\n          \"default\": \"tsc\",\n  \
  \        \"description\": \"Builder to use for compilation\"\n        },\n        \"typeCheck\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Enable type checking (when using SWC builder)\"\n        }\n      }\n    },\n    \"generateOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Default options for nest generate command\",\n      \"properties\": {\n        \"spec\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Generate spec/test files\"\n        },\n        \"flat\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Generate without subdirectory\"\n        },\n        \"baseDir\": {\n          \"type\": \"string\",\n          \"description\": \"Base directory for generating\"\n        }\n      }\n    },\n    \"projects\": {\n      \"type\": \"object\",\n      \"description\": \"Projects in a monorepo workspace\",\n  \
  \    \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"application\", \"library\"],\n            \"description\": \"Project type\"\n          },\n          \"root\": {\n            \"type\": \"string\",\n            \"description\": \"Project root directory\"\n          },\n          \"entryFile\": {\n            \"type\": \"string\",\n            \"default\": \"main\",\n            \"description\": \"Entry file for the project\"\n          },\n          \"sourceRoot\": {\n            \"type\": \"string\",\n            \"description\": \"Source root for the project\"\n          },\n          \"compilerOptions\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"tsConfigPath\": { \"type\": \"string\" },\n              \"webpack\": { \"type\": \"boolean\" }\n            }\n          }\n        },\n        \"required\": [\"type\", \"root\"\
  , \"sourceRoot\"]\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nestjs/refs/heads/main/json-schema/nest-cli-config.json
tags:
- Frameworks
- GraphQL
- Microservices
- Node.js
- REST
- TypeScript
- WebSockets
title: NestJS CLI Configuration (nest-cli.json)
---
