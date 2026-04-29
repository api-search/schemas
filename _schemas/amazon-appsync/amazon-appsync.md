---
description: Schema defining the structure of an Amazon AppSync GraphQL API resource, including authentication configuration, data sources, resolvers, types, and API settings.
layout: schema
name: Amazon AppSync GraphQL API
properties_list:
- description: The unique identifier for the GraphQL API.
  name: apiId
  type: string
- description: The name of the GraphQL API.
  name: name
  type: string
- description: The authentication type for the GraphQL API.
  name: authenticationType
  type: string
- description: The ARN of the GraphQL API.
  name: arn
  type: string
- description: The URIs associated with the GraphQL API.
  name: uris
  type: object
- description: ''
  name: logConfig
  type: object
- description: ''
  name: userPoolConfig
  type: object
- description: ''
  name: openIDConnectConfig
  type: object
- description: ''
  name: lambdaAuthorizerConfig
  type: object
- description: A list of additional authentication providers for the GraphQL API.
  name: additionalAuthenticationProviders
  type: array
- description: Whether AWS X-Ray tracing is enabled for this API.
  name: xrayEnabled
  type: boolean
- description: The ARN of the AWS WAF web ACL associated with this API.
  name: wafWebAclArn
  type: string
- description: Tags for the GraphQL API.
  name: tags
  type: object
- description: The data sources configured for the GraphQL API.
  name: dataSources
  type: array
- description: The resolvers configured for the GraphQL API.
  name: resolvers
  type: array
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/amazon-appsync-schema.json
slug: amazon-appsync
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-appsync/graphql-api\",\n  \"title\": \"Amazon AppSync GraphQL API\",\n  \"description\": \"Schema defining the structure of an Amazon AppSync GraphQL API resource, including authentication configuration, data sources, resolvers, types, and API settings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"authenticationType\"\n  ],\n  \"properties\": {\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the GraphQL API.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the GraphQL API.\",\n      \"minLength\": 1,\n      \"maxLength\": 128\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"API_KEY\",\n        \"AWS_IAM\",\n        \"AMAZON_COGNITO_USER_POOLS\",\n        \"OPENID_CONNECT\",\n        \"AWS_LAMBDA\"\
  \n      ],\n      \"description\": \"The authentication type for the GraphQL API.\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the GraphQL API.\"\n    },\n    \"uris\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The URIs associated with the GraphQL API.\"\n    },\n    \"logConfig\": {\n      \"$ref\": \"#/$defs/LogConfig\"\n    },\n    \"userPoolConfig\": {\n      \"$ref\": \"#/$defs/UserPoolConfig\"\n    },\n    \"openIDConnectConfig\": {\n      \"$ref\": \"#/$defs/OpenIDConnectConfig\"\n    },\n    \"lambdaAuthorizerConfig\": {\n      \"$ref\": \"#/$defs/LambdaAuthorizerConfig\"\n    },\n    \"additionalAuthenticationProviders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AdditionalAuthenticationProvider\"\n      },\n      \"description\": \"A list of additional authentication providers for the GraphQL API.\"\n   \
  \ },\n    \"xrayEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether AWS X-Ray tracing is enabled for this API.\"\n    },\n    \"wafWebAclArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the AWS WAF web ACL associated with this API.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for the GraphQL API.\"\n    },\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DataSource\"\n      },\n      \"description\": \"The data sources configured for the GraphQL API.\"\n    },\n    \"resolvers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Resolver\"\n      },\n      \"description\": \"The resolvers configured for the GraphQL API.\"\n    }\n  },\n  \"$defs\": {\n    \"LogConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The Amazon CloudWatch\
  \ Logs configuration.\",\n      \"required\": [\n        \"cloudWatchLogsRoleArn\",\n        \"fieldLogLevel\"\n      ],\n      \"properties\": {\n        \"fieldLogLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"NONE\",\n            \"ERROR\",\n            \"ALL\"\n          ]\n        },\n        \"cloudWatchLogsRoleArn\": {\n          \"type\": \"string\"\n        },\n        \"excludeVerboseContent\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"UserPoolConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The Amazon Cognito user pool configuration.\",\n      \"required\": [\n        \"userPoolId\",\n        \"awsRegion\",\n        \"defaultAction\"\n      ],\n      \"properties\": {\n        \"userPoolId\": {\n          \"type\": \"string\"\n        },\n        \"awsRegion\": {\n          \"type\": \"string\"\n        },\n        \"defaultAction\": {\n          \"type\": \"string\",\n          \"enum\": [\n  \
  \          \"ALLOW\",\n            \"DENY\"\n          ]\n        },\n        \"appIdClientRegex\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"OpenIDConnectConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The OpenID Connect configuration.\",\n      \"required\": [\n        \"issuer\"\n      ],\n      \"properties\": {\n        \"issuer\": {\n          \"type\": \"string\"\n        },\n        \"clientId\": {\n          \"type\": \"string\"\n        },\n        \"iatTTL\": {\n          \"type\": \"integer\"\n        },\n        \"authTTL\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"LambdaAuthorizerConfig\": {\n      \"type\": \"object\",\n      \"description\": \"A Lambda function used for authorization.\",\n      \"required\": [\n        \"authorizerUri\"\n      ],\n      \"properties\": {\n        \"authorizerResultTtlInSeconds\": {\n          \"type\": \"integer\"\n        },\n        \"authorizerUri\": {\n     \
  \     \"type\": \"string\"\n        },\n        \"identityValidationExpression\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"AdditionalAuthenticationProvider\": {\n      \"type\": \"object\",\n      \"description\": \"An additional authentication provider.\",\n      \"required\": [\n        \"authenticationType\"\n      ],\n      \"properties\": {\n        \"authenticationType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"API_KEY\",\n            \"AWS_IAM\",\n            \"AMAZON_COGNITO_USER_POOLS\",\n            \"OPENID_CONNECT\",\n            \"AWS_LAMBDA\"\n          ]\n        },\n        \"openIDConnectConfig\": {\n          \"$ref\": \"#/$defs/OpenIDConnectConfig\"\n        },\n        \"userPoolConfig\": {\n          \"type\": \"object\"\n        },\n        \"lambdaAuthorizerConfig\": {\n          \"$ref\": \"#/$defs/LambdaAuthorizerConfig\"\n        }\n      }\n    },\n    \"DataSource\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"A data source in AppSync that resolvers can connect to.\",\n      \"required\": [\n        \"name\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"dataSourceArn\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"AWS_LAMBDA\",\n            \"AMAZON_DYNAMODB\",\n            \"AMAZON_ELASTICSEARCH\",\n            \"AMAZON_OPENSEARCH_SERVICE\",\n            \"HTTP\",\n            \"RELATIONAL_DATABASE\",\n            \"NONE\",\n            \"AMAZON_EVENTBRIDGE\"\n          ]\n        },\n        \"serviceRoleArn\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Resolver\": {\n      \"type\": \"object\",\n      \"description\": \"A resolver maps a GraphQL operation to a data source.\",\n      \"required\"\
  : [\n        \"typeName\",\n        \"fieldName\"\n      ],\n      \"properties\": {\n        \"typeName\": {\n          \"type\": \"string\"\n        },\n        \"fieldName\": {\n          \"type\": \"string\"\n        },\n        \"dataSourceName\": {\n          \"type\": \"string\"\n        },\n        \"resolverArn\": {\n          \"type\": \"string\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"UNIT\",\n            \"PIPELINE\"\n          ]\n        },\n        \"requestMappingTemplate\": {\n          \"type\": \"string\"\n        },\n        \"responseMappingTemplate\": {\n          \"type\": \"string\"\n        },\n        \"pipelineConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"functions\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/amazon-appsync-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: Amazon AppSync GraphQL API
---
