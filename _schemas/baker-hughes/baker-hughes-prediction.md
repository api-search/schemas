---
description: AI-generated predictive maintenance forecast from Baker Hughes BHC3 AI Suite.
layout: schema
name: Prediction
properties_list:
- description: Unique identifier for the prediction.
  name: predictionId
  type: string
- description: Identifier of the asset this prediction applies to.
  name: assetId
  type: string
- description: Category of prediction.
  name: predictionType
  type: string
- description: Probability of failure in the next prediction window (0.0 to 1.0).
  name: failureProbability
  type: number
- description: Estimated time until failure expressed as ISO 8601 duration (e.g., P7D for 7 days).
  name: estimatedTimeToFailure
  type: string
- description: Model confidence in this prediction (0.0 to 1.0).
  name: confidenceScore
  type: number
- description: Recommended maintenance or operational action.
  name: recommendedAction
  type: string
- description: Timestamp when this prediction was generated.
  name: generatedAt
  type: string
provider_name: Baker Hughes
provider_slug: baker-hughes
schema_file: json-schema/baker-hughes-prediction-schema.json
slug: baker-hughes-prediction
tags:
- Energy Technology
- Industrial IoT
- Oil And Gas
- Asset Performance Management
- Digital Energy
title: Prediction
---
