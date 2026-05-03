---
description: Represents a prediction result from Salesforce Einstein, including score, label, and explanatory factors.
layout: schema
name: Einstein Prediction
properties_list:
- description: Unique prediction identifier.
  name: id
  type: string
- description: ID of the prediction definition that generated this prediction.
  name: predictionDefinitionId
  type: string
- description: Salesforce record ID the prediction applies to.
  name: recordId
  type: string
- description: Prediction confidence score, typically between 0.0 and 1.0.
  name: score
  type: number
- description: Predicted label for categorical predictions.
  name: label
  type: string
- description: Type of prediction.
  name: predictionType
  type: string
- description: Predicted numeric value for numeric predictions.
  name: numericValue
  type: number
- description: Top factors influencing the prediction.
  name: factors
  type: array
- description: Recommended actions to improve the predicted outcome.
  name: prescriptions
  type: array
- description: ID of the model used for the prediction.
  name: modelId
  type: string
- description: Timestamp when the prediction was generated.
  name: createdDate
  type: string
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
schema_file: json-schema/salesforce-einstein-prediction-schema.json
slug: salesforce-einstein-prediction
source_filename: salesforce-einstein-prediction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/salesforce-einstein/json-schema/salesforce-einstein-prediction-schema.json\",\n  \"title\": \"Einstein Prediction\",\n  \"description\": \"Represents a prediction result from Salesforce Einstein, including score, label, and explanatory factors.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique prediction identifier.\"\n    },\n    \"predictionDefinitionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the prediction definition that generated this prediction.\"\n    },\n    \"recordId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID the prediction applies to.\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Prediction confidence score, typically between 0.0 and 1.0.\",\n      \"minimum\": 0,\n      \"maximum\"\
  : 1\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Predicted label for categorical predictions.\"\n    },\n    \"predictionType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of prediction.\",\n      \"enum\": [\"Boolean\", \"Categorical\", \"Numeric\"]\n    },\n    \"numericValue\": {\n      \"type\": \"number\",\n      \"description\": \"Predicted numeric value for numeric predictions.\"\n    },\n    \"factors\": {\n      \"type\": \"array\",\n      \"description\": \"Top factors influencing the prediction.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PredictionFactor\"\n      }\n    },\n    \"prescriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Recommended actions to improve the predicted outcome.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Prescription\"\n      }\n    },\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the model used for the prediction.\"\n    },\n\
  \    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the prediction was generated.\"\n    }\n  },\n  \"required\": [\"predictionDefinitionId\", \"score\"],\n  \"$defs\": {\n    \"PredictionFactor\": {\n      \"type\": \"object\",\n      \"description\": \"A factor that influenced the prediction outcome.\",\n      \"properties\": {\n        \"featureName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the feature or field.\"\n        },\n        \"featureValue\": {\n          \"type\": \"string\",\n          \"description\": \"Value of the feature for this prediction.\"\n        },\n        \"importance\": {\n          \"type\": \"number\",\n          \"description\": \"Importance weight of the factor.\"\n        },\n        \"direction\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the factor positively or negatively affects the prediction.\",\n          \"\
  enum\": [\"Positive\", \"Negative\"]\n        }\n      },\n      \"required\": [\"featureName\", \"importance\"]\n    },\n    \"Prescription\": {\n      \"type\": \"object\",\n      \"description\": \"A recommended action to improve the predicted outcome.\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\",\n          \"description\": \"Recommended action to take.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Detailed description of the recommendation.\"\n        },\n        \"impact\": {\n          \"type\": \"number\",\n          \"description\": \"Expected impact of the action on the outcome.\"\n        }\n      },\n      \"required\": [\"action\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/json-schema/salesforce-einstein-prediction-schema.json
tags:
- Artificial Intelligence
- Computer Vision
- CRM
- Machine Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
title: Einstein Prediction
---
