---
description: ''
layout: schema
name: Capabilities
properties_list:
- description: ''
  name: associatedActions
  type: object
- description: ''
  name: bookmarks
  type: object
- description: ''
  name: chatterLikes
  type: object
- description: ''
  name: close
  type: object
- description: ''
  name: comments
  type: object
- description: ''
  name: edit
  type: object
- description: ''
  name: interactions
  type: object
- description: ''
  name: mute
  type: object
- description: ''
  name: readBy
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: topics
  type: object
- description: ''
  name: upDownVote
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-capabilities-schema.json
slug: salesforce-capabilities
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"associatedActions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"platformActionGroups\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"platformActionGroups\"\n      ]\n    },\n    \"bookmarks\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isBookmarkedByCurrentUser\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"isBookmarkedByCurrentUser\"\n      ]\n    },\n    \"chatterLikes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isLikedByCurrentUser\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"likesMessage\": {\n          \"type\": \"['string', 'null']\",\n          \"\
  example\": \"example_value\"\n        },\n        \"myLike\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"page\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"currentPageToken\": {\n              \"type\": \"integer\",\n              \"example\": \"CAUQAA\"\n            },\n            \"currentPageUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"items\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"nextPageToken\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"nextPageUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"\
  https://www.example.com\"\n            },\n            \"previousPageToken\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"previousPageUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"total\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            }\n          },\n          \"required\": [\n            \"currentPageToken\",\n            \"currentPageUrl\",\n            \"items\",\n            \"nextPageToken\",\n            \"nextPageUrl\",\n            \"previousPageToken\",\n            \"previousPageUrl\",\n            \"total\"\n          ]\n        }\n      },\n      \"required\": [\n        \"isLikedByCurrentUser\",\n        \"likesMessage\",\n        \"myLike\",\n        \"page\"\n      ]\n    },\n    \"close\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"canContextUserUpdateIsClosed\"\
  : {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isClosed\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"canContextUserUpdateIsClosed\",\n        \"isClosed\"\n      ]\n    },\n    \"comments\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"page\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"currentPageToken\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"currentPageUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"items\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"nextPageToken\": {\n\
  \              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"nextPageUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"previousPageToken\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"previousPageUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"total\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            }\n          },\n          \"required\": [\n            \"currentPageToken\",\n            \"currentPageUrl\",\n            \"items\",\n            \"nextPageToken\",\n            \"nextPageUrl\",\n            \"previousPageToken\",\n            \"previousPageUrl\",\n            \"total\"\n          ]\n        }\n      },\n      \"required\"\
  : [\n        \"page\"\n      ]\n    },\n    \"edit\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isEditRestricted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isEditableByMeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"lastEditedBy\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"lastEditedDate\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"latestRevision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"relativeLastEditedDate\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"isEditRestricted\",\n        \"isEditableByMeUrl\",\n        \"lastEditedBy\",\n        \"lastEditedDate\",\n\
  \        \"latestRevision\",\n        \"relativeLastEditedDate\"\n      ]\n    },\n    \"interactions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        }\n      },\n      \"required\": [\n        \"count\"\n      ]\n    },\n    \"mute\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isMutedByMe\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"isMutedByMe\"\n      ]\n    },\n    \"readBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isReadByMe\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"lastReadDateByMe\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"page\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"currentPageToken\": {\n           \
  \   \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"currentPageUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"items\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"nextPageToken\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"nextPageUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"previousPageToken\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"CAUQAA\"\n            },\n            \"previousPageUrl\": {\n              \"type\": \"['string', 'null']\",\n            \
  \  \"example\": \"https://www.example.com\"\n            },\n            \"total\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            }\n          },\n          \"required\": [\n            \"currentPageToken\",\n            \"currentPageUrl\",\n            \"items\",\n            \"nextPageToken\",\n            \"nextPageUrl\",\n            \"previousPageToken\",\n            \"previousPageUrl\",\n            \"total\"\n          ]\n        }\n      },\n      \"required\": [\n        \"isReadByMe\",\n        \"lastReadDateByMe\",\n        \"page\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"feedEntityStatus\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"isApprovableByMe\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"feedEntityStatus\",\n        \"isApprovableByMe\"\n\
  \      ]\n    },\n    \"topics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"canAssignTopics\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"canAssignTopics\",\n        \"items\"\n      ]\n    },\n    \"upDownVote\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"downVoteCount\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"myVote\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"upVoteCount\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        }\n      },\n      \"required\": [\n        \"downVoteCount\",\n        \"myVote\",\n        \"upVoteCount\"\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"associatedActions\",\n    \"bookmarks\",\n    \"chatterLikes\",\n    \"close\",\n    \"comments\",\n    \"edit\",\n    \"interactions\",\n    \"mute\",\n    \"readBy\",\n    \"status\",\n    \"topics\",\n    \"upDownVote\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Capabilities\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-capabilities-schema.json
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
title: Capabilities
---
