---
description: Provides information about Amazon Pinpoint configuration settings for retrieving and processing data from a recommender model.
layout: schema
name: RecommenderConfigurationResponse
properties_list:
- description: ''
  name: Attributes
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RecommendationProviderIdType
  type: object
- description: ''
  name: RecommendationProviderRoleArn
  type: object
- description: ''
  name: RecommendationProviderUri
  type: object
- description: ''
  name: RecommendationTransformerUri
  type: object
- description: ''
  name: RecommendationsDisplayName
  type: object
- description: ''
  name: RecommendationsPerMessage
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-recommender-configuration-response-schema.json
slug: amazon-pinpoint-recommender-configuration-response
source_filename: amazon-pinpoint-recommender-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-recommender-configuration-response-schema.json\",\n  \"title\": \"RecommenderConfigurationResponse\",\n  \"description\": \"Provides information about Amazon Pinpoint configuration settings for retrieving and processing data from a recommender model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"<p>A map that defines 1-10 custom endpoint or user attributes, depending on the value for the RecommendationProviderIdType property. Each of these attributes temporarily stores a recommended item that's retrieved from the recommender model and sent to an AWS Lambda function for additional processing. Each attribute can be used as\
  \ a message variable in a message template.</p> <p>This value is null if the configuration doesn't invoke an AWS Lambda function (RecommendationTransformerUri) to perform additional processing of recommendation data.</p>\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in extended ISO 8601 format, when the configuration was created for the recommender model.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the configuration for the recommender model.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the recommender\
  \ model configuration.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in extended ISO 8601 format, when the configuration for the recommender model was last modified.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the configuration for the recommender model.\"\n        }\n      ]\n    },\n    \"RecommendationProviderIdType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The type of Amazon Pinpoint ID that's associated with unique user IDs in the recommender model. This value enables the model to use attribute and event data that\\u2019s specific to a particular endpoint or user\
  \ in an Amazon Pinpoint application. Possible values are:</p> <ul><li><p>PINPOINT_ENDPOINT_ID - Each user in the model is associated with a particular endpoint in Amazon Pinpoint. The data is correlated based on endpoint IDs in Amazon Pinpoint. This is the default value.</p></li> <li><p>PINPOINT_USER_ID - Each user in the model is associated with a particular user and endpoint in Amazon Pinpoint. The data is correlated based on user IDs in Amazon Pinpoint. If this value is specified, an endpoint definition in Amazon Pinpoint has to specify both a user ID (UserId) and an endpoint ID. Otherwise, messages won\\u2019t be sent to the user's endpoint.</p></li></ul>\"\n        }\n      ]\n    },\n    \"RecommendationProviderRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Identity and Access Management (IAM) role that authorizes Amazon Pinpoint to retrieve\
  \ recommendation data from the recommender model.\"\n        }\n      ]\n    },\n    \"RecommendationProviderUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the recommender model that Amazon Pinpoint retrieves the recommendation data from. This value is the ARN of an Amazon Personalize campaign.\"\n        }\n      ]\n    },\n    \"RecommendationTransformerUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name or Amazon Resource Name (ARN) of the AWS Lambda function that Amazon Pinpoint invokes to perform additional processing of recommendation data that it retrieves from the recommender model.\"\n        }\n      ]\n    },\n    \"RecommendationsDisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n     \
  \   },\n        {\n          \"description\": \"<p>The custom display name for the standard endpoint or user attribute (RecommendationItems) that temporarily stores recommended items for each endpoint or user, depending on the value for the RecommendationProviderIdType property. This name appears in the <b>Attribute finder</b> of the template editor on the Amazon Pinpoint console.</p> <p>This value is null if the configuration doesn't invoke an AWS Lambda function (RecommendationTransformerUri) to perform additional processing of recommendation data.</p>\"\n        }\n      ]\n    },\n    \"RecommendationsPerMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The number of recommended items that are retrieved from the model for each endpoint or user, depending on the value for the RecommendationProviderIdType property. This number determines how many recommended items are available for\
  \ use in message variables.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecommendationProviderUri\",\n    \"LastModifiedDate\",\n    \"CreationDate\",\n    \"RecommendationProviderRoleArn\",\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-recommender-configuration-response-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: RecommenderConfigurationResponse
---
