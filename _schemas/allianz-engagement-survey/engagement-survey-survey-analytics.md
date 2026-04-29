---
description: Aggregated analytics and insights for an engagement survey
layout: schema
name: SurveyAnalytics
properties_list:
- description: Survey being analyzed
  name: survey_id
  type: string
- description: Percentage of invited employees who responded
  name: participation_rate
  type: number
- description: Overall engagement score out of 100
  name: engagement_score
  type: number
- description: Percentage of favorable responses across all questions
  name: favorable_percentage
  type: number
- description: Per-question score breakdown
  name: question_scores
  type: array
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-survey-analytics-schema.json
slug: engagement-survey-survey-analytics
source_filename: engagement-survey-survey-analytics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-analytics-schema.json\",\n  \"title\": \"SurveyAnalytics\",\n  \"description\": \"Aggregated analytics and insights for an engagement survey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"survey_id\": {\n      \"type\": \"string\",\n      \"description\": \"Survey being analyzed\",\n      \"example\": \"survey-500123\"\n    },\n    \"participation_rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Percentage of invited employees who responded\",\n      \"example\": 70.1\n    },\n    \"engagement_score\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Overall engagement score out of 100\",\n      \"example\": 76.3\n    },\n    \"favorable_percentage\": {\n      \"type\": \"number\"\
  ,\n      \"format\": \"double\",\n      \"description\": \"Percentage of favorable responses across all questions\",\n      \"example\": 74.8\n    },\n    \"question_scores\": {\n      \"type\": \"array\",\n      \"description\": \"Per-question score breakdown\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/QuestionScore\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-analytics-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: SurveyAnalytics
---
