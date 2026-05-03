---
description: Represents a news article or headline from the Refinitiv Data Platform News API, including metadata, content, and classification information.
layout: schema
name: Refinitiv News Article
properties_list:
- description: Unique identifier for the news story.
  name: storyId
  type: string
- description: The headline text of the news article.
  name: title
  type: string
- description: The full text body of the news article, available when retrieving the complete story.
  name: body
  type:
  - string
  - 'null'
- description: Timestamp when the article was originally created or published.
  name: versionCreated
  type: string
- description: Timestamp of the first version of the story.
  name: firstCreated
  type:
  - string
  - 'null'
- description: Code identifying the news source such as NS:RTRS for Reuters.
  name: sourceCode
  type:
  - string
  - 'null'
- description: Human-readable name of the news source.
  name: sourceName
  type:
  - string
  - 'null'
- description: ISO 639-1 language code of the article.
  name: language
  type:
  - string
  - 'null'
- description: The urgency level of the news, with lower values indicating higher urgency.
  name: urgency
  type:
  - integer
  - 'null'
- description: Subject classification codes for the article.
  name: subjects
  type:
  - array
  - 'null'
- description: Target audience codes for the article.
  name: audiences
  type:
  - array
  - 'null'
- description: Financial instruments referenced in the article.
  name: instruments
  type:
  - array
  - 'null'
- description: A reference identifier for the news item.
  name: newsItem
  type:
  - string
  - 'null'
provider_name: Refinitiv
provider_slug: refinitiv
schema_file: json-schema/refinitiv-news-article-schema.json
slug: refinitiv-news-article
source_filename: refinitiv-news-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.refinitiv.com/schemas/refinitiv/news-article.json\",\n  \"title\": \"Refinitiv News Article\",\n  \"description\": \"Represents a news article or headline from the Refinitiv Data Platform News API, including metadata, content, and classification information.\",\n  \"type\": \"object\",\n  \"required\": [\"storyId\", \"title\", \"versionCreated\"],\n  \"properties\": {\n    \"storyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the news story.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The headline text of the news article.\"\n    },\n    \"body\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The full text body of the news article, available when retrieving the complete story.\"\n    },\n    \"versionCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"Timestamp when the article was originally created or published.\"\n    },\n    \"firstCreated\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the first version of the story.\"\n    },\n    \"sourceCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Code identifying the news source such as NS:RTRS for Reuters.\"\n    },\n    \"sourceName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Human-readable name of the news source.\"\n    },\n    \"language\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ISO 639-1 language code of the article.\",\n      \"pattern\": \"^[a-z]{2}$\"\n    },\n    \"urgency\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The urgency level of the news, with lower values indicating higher urgency.\",\n      \"minimum\": 1\n    },\n    \"subjects\": {\n      \"type\": [\"array\", \"null\"\
  ],\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Subject classification codes for the article.\"\n    },\n    \"audiences\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Target audience codes for the article.\"\n    },\n    \"instruments\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ric\": {\n            \"type\": \"string\",\n            \"description\": \"RIC of the related instrument.\"\n          },\n          \"name\": {\n            \"type\": [\"string\", \"null\"],\n            \"description\": \"Name of the related instrument.\"\n          }\n        }\n      },\n      \"description\": \"Financial instruments referenced in the article.\"\n    },\n    \"newsItem\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A reference identifier for the news item.\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/json-schema/refinitiv-news-article-schema.json
tags: []
title: Refinitiv News Article
---
