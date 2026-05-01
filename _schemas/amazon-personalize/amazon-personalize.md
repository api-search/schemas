---
description: Schema defining the structure of an Amazon Personalize dataset group resource, including datasets, solutions, campaigns, and recommenders for building personalized recommendation systems.
layout: schema
name: Amazon Personalize Dataset Group Definition
properties_list:
- description: The name of the dataset group.
  name: name
  type: string
- description: The Amazon Resource Name of the dataset group.
  name: datasetGroupArn
  type: string
- description: The current status of the dataset group.
  name: status
  type: string
- description: The domain of the dataset group for domain-based recommenders.
  name: domain
  type: string
- description: The ARN of the KMS key used to encrypt the datasets.
  name: kmsKeyArn
  type: string
- description: The ARN of the IAM role that has permissions to access the datasets.
  name: roleArn
  type: string
- description: The creation date and time of the dataset group.
  name: creationDateTime
  type: string
- description: The last updated date and time of the dataset group.
  name: lastUpdatedDateTime
  type: string
- description: The datasets in the dataset group.
  name: datasets
  type: array
- description: The trained solutions in the dataset group.
  name: solutions
  type: array
- description: The deployed campaigns for real-time recommendations.
  name: campaigns
  type: array
- description: Domain-based recommenders in the dataset group.
  name: recommenders
  type: array
provider_name: Amazon Personalize
provider_slug: amazon-personalize
schema_file: json-schema/amazon-personalize-schema.json
slug: amazon-personalize
source_filename: amazon-personalize-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-personalize/dataset-group-definition\",\n  \"title\": \"Amazon Personalize Dataset Group Definition\",\n  \"description\": \"Schema defining the structure of an Amazon Personalize dataset group resource, including datasets, solutions, campaigns, and recommenders for building personalized recommendation systems.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dataset group.\",\n      \"minLength\": 1,\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9_-]*$\"\n    },\n    \"datasetGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name of the dataset group.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the dataset\
  \ group.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ECOMMERCE\",\n        \"VIDEO_ON_DEMAND\"\n      ],\n      \"description\": \"The domain of the dataset group for domain-based recommenders.\"\n    },\n    \"kmsKeyArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the KMS key used to encrypt the datasets.\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role that has permissions to access the datasets.\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation date and time of the dataset group.\"\n    },\n    \"lastUpdatedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last updated date and time of the dataset group.\"\n    },\n    \"datasets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Dataset\"\
  \n      },\n      \"description\": \"The datasets in the dataset group.\"\n    },\n    \"solutions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Solution\"\n      },\n      \"description\": \"The trained solutions in the dataset group.\"\n    },\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Campaign\"\n      },\n      \"description\": \"The deployed campaigns for real-time recommendations.\"\n    },\n    \"recommenders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Recommender\"\n      },\n      \"description\": \"Domain-based recommenders in the dataset group.\"\n    }\n  },\n  \"$defs\": {\n    \"Dataset\": {\n      \"type\": \"object\",\n      \"description\": \"A dataset containing interaction, user, or item data for training.\",\n      \"required\": [\n        \"name\",\n        \"datasetType\"\n      ],\n      \"properties\": {\n        \"name\": {\n       \
  \   \"type\": \"string\",\n          \"description\": \"The name of the dataset.\"\n        },\n        \"datasetArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the dataset.\"\n        },\n        \"datasetGroupArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the dataset group.\"\n        },\n        \"datasetType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Interactions\",\n            \"Items\",\n            \"Users\",\n            \"Actions\",\n            \"Action_Interactions\"\n          ],\n          \"description\": \"The type of dataset.\"\n        },\n        \"schemaArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the schema associated with the dataset.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the dataset.\"\n        },\n        \"creationDateTime\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"Solution\": {\n      \"type\": \"object\",\n      \"description\": \"A trained model that generates recommendations.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the solution.\"\n        },\n        \"solutionArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the solution.\"\n        },\n        \"recipeArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the recipe used to create the solution.\"\n        },\n        \"datasetGroupArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the dataset group that provides the training data.\"\n        },\n        \"performAutoML\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to perform automated ML to find the best\
  \ recipe.\"\n        },\n        \"performHPO\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to perform hyperparameter optimization.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the solution.\"\n        },\n        \"solutionConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"eventValueThreshold\": {\n              \"type\": \"string\"\n            },\n            \"algorithmHyperParameters\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            },\n            \"featureTransformationParameters\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Campaign\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A deployed solution version for real-time recommendations.\",\n      \"required\": [\n        \"name\",\n        \"solutionVersionArn\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the campaign.\"\n        },\n        \"campaignArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the campaign.\"\n        },\n        \"solutionVersionArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the deployed solution version.\"\n        },\n        \"minProvisionedTPS\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The minimum provisioned transactions per second.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the campaign.\"\n        },\n        \"creationDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  \n        }\n      }\n    },\n    \"Recommender\": {\n      \"type\": \"object\",\n      \"description\": \"A domain-based recommender for specific use cases.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the recommender.\"\n        },\n        \"recommenderArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the recommender.\"\n        },\n        \"datasetGroupArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the dataset group.\"\n        },\n        \"recipeArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the recipe for the recommender.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the recommender.\"\n        },\n        \"creationDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/amazon-personalize-schema.json
tags:
- AI
- Customer Experience
- Machine Learning
- ML
- Personalization
- Recommendations
title: Amazon Personalize Dataset Group Definition
---
