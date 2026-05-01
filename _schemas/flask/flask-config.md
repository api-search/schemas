---
description: JSON Schema for Flask application configuration values, covering core settings, session, security, template, and common extension configuration.
layout: schema
name: Flask Application Configuration
properties_list:
- description: Enable debug mode.
  name: DEBUG
  type: boolean
- description: Enable testing mode.
  name: TESTING
  type: boolean
- description: Secret key for session signing and CSRF protection.
  name: SECRET_KEY
  type: string
- description: Application environment (deprecated in Flask 2.3+).
  name: ENV
  type: string
- description: Server name for URL generation (host:port).
  name: SERVER_NAME
  type: string
- description: Application root path.
  name: APPLICATION_ROOT
  type: string
- description: URL scheme for URL generation.
  name: PREFERRED_URL_SCHEME
  type: string
- description: Maximum request content length in bytes.
  name: MAX_CONTENT_LENGTH
  type: integer
- description: Maximum cookie size warning threshold.
  name: MAX_COOKIE_SIZE
  type: integer
- description: Name of the session cookie.
  name: SESSION_COOKIE_NAME
  type: string
- description: Domain for the session cookie.
  name: SESSION_COOKIE_DOMAIN
  type: string
- description: Path for the session cookie.
  name: SESSION_COOKIE_PATH
  type: string
- description: Set HttpOnly flag on session cookie.
  name: SESSION_COOKIE_HTTPONLY
  type: boolean
- description: Set Secure flag on session cookie.
  name: SESSION_COOKIE_SECURE
  type: boolean
- description: SameSite attribute for session cookie.
  name: SESSION_COOKIE_SAMESITE
  type: string
- description: Permanent session lifetime in seconds.
  name: PERMANENT_SESSION_LIFETIME
  type: integer
- description: Refresh cookie on each request.
  name: SESSION_REFRESH_EACH_REQUEST
  type: boolean
- description: Sort keys in JSON responses.
  name: JSON_SORT_KEYS
  type: boolean
- description: MIME type for jsonify responses.
  name: JSONIFY_MIMETYPE
  type: string
- description: Auto-reload templates on change.
  name: TEMPLATES_AUTO_RELOAD
  type: boolean
- description: Log template loading for debugging.
  name: EXPLAIN_TEMPLATE_LOADING
  type: boolean
- description: Trap HTTP exceptions for debugging.
  name: TRAP_HTTP_EXCEPTIONS
  type: boolean
- description: Trap bad request errors.
  name: TRAP_BAD_REQUEST_ERRORS
  type: boolean
- description: Propagate exceptions instead of handling.
  name: PROPAGATE_EXCEPTIONS
  type: boolean
- description: SQLAlchemy database connection URI (Flask-SQLAlchemy extension).
  name: SQLALCHEMY_DATABASE_URI
  type: string
- description: Track SQLAlchemy model modifications.
  name: SQLALCHEMY_TRACK_MODIFICATIONS
  type: boolean
- description: Echo SQL statements.
  name: SQLALCHEMY_ECHO
  type: boolean
- description: Connection pool size.
  name: SQLALCHEMY_POOL_SIZE
  type: integer
- description: Pool checkout timeout in seconds.
  name: SQLALCHEMY_POOL_TIMEOUT
  type: integer
- description: Max connections beyond pool size.
  name: SQLALCHEMY_MAX_OVERFLOW
  type: integer
- description: Mail server hostname (Flask-Mail extension).
  name: MAIL_SERVER
  type: string
- description: Mail server port.
  name: MAIL_PORT
  type: integer
- description: Use TLS for mail.
  name: MAIL_USE_TLS
  type: boolean
- description: Use SSL for mail.
  name: MAIL_USE_SSL
  type: boolean
- description: Mail server username.
  name: MAIL_USERNAME
  type: string
- description: Mail server password.
  name: MAIL_PASSWORD
  type: string
- description: Cache backend type (Flask-Caching extension).
  name: CACHE_TYPE
  type: string
- description: Default cache timeout in seconds.
  name: CACHE_DEFAULT_TIMEOUT
  type: integer
- description: Redis URL for cache backend.
  name: CACHE_REDIS_URL
  type: string
- description: Allowed origins for CORS (Flask-CORS extension).
  name: CORS_ORIGINS
  type: array
- description: Allowed HTTP methods for CORS.
  name: CORS_METHODS
  type: array
- description: Allow credentials in CORS requests.
  name: CORS_SUPPORTS_CREDENTIALS
  type: boolean
provider_name: Flask
provider_slug: flask
schema_file: json-schema/flask-config.json
slug: flask-config
source_filename: flask-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/flask/json-schema/flask-config.json\",\n  \"title\": \"Flask Application Configuration\",\n  \"description\": \"JSON Schema for Flask application configuration values, covering core settings, session, security, template, and common extension configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DEBUG\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable debug mode.\",\n      \"default\": false\n    },\n    \"TESTING\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable testing mode.\",\n      \"default\": false\n    },\n    \"SECRET_KEY\": {\n      \"type\": \"string\",\n      \"description\": \"Secret key for session signing and CSRF protection.\"\n    },\n    \"ENV\": {\n      \"type\": \"string\",\n      \"description\": \"Application environment (deprecated in Flask 2.3+).\",\n      \"enum\": [\"production\", \"\
  development\", \"testing\"],\n      \"default\": \"production\"\n    },\n    \"SERVER_NAME\": {\n      \"type\": \"string\",\n      \"description\": \"Server name for URL generation (host:port).\"\n    },\n    \"APPLICATION_ROOT\": {\n      \"type\": \"string\",\n      \"description\": \"Application root path.\",\n      \"default\": \"/\"\n    },\n    \"PREFERRED_URL_SCHEME\": {\n      \"type\": \"string\",\n      \"description\": \"URL scheme for URL generation.\",\n      \"enum\": [\"http\", \"https\"],\n      \"default\": \"http\"\n    },\n    \"MAX_CONTENT_LENGTH\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum request content length in bytes.\"\n    },\n    \"MAX_COOKIE_SIZE\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum cookie size warning threshold.\",\n      \"default\": 4093\n    },\n    \"SESSION_COOKIE_NAME\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the session cookie.\",\n      \"default\": \"session\"\n   \
  \ },\n    \"SESSION_COOKIE_DOMAIN\": {\n      \"type\": \"string\",\n      \"description\": \"Domain for the session cookie.\"\n    },\n    \"SESSION_COOKIE_PATH\": {\n      \"type\": \"string\",\n      \"description\": \"Path for the session cookie.\",\n      \"default\": \"/\"\n    },\n    \"SESSION_COOKIE_HTTPONLY\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set HttpOnly flag on session cookie.\",\n      \"default\": true\n    },\n    \"SESSION_COOKIE_SECURE\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set Secure flag on session cookie.\",\n      \"default\": false\n    },\n    \"SESSION_COOKIE_SAMESITE\": {\n      \"type\": \"string\",\n      \"description\": \"SameSite attribute for session cookie.\",\n      \"enum\": [\"Strict\", \"Lax\", \"None\"],\n      \"default\": \"Lax\"\n    },\n    \"PERMANENT_SESSION_LIFETIME\": {\n      \"type\": \"integer\",\n      \"description\": \"Permanent session lifetime in seconds.\",\n      \"default\": 2678400\n\
  \    },\n    \"SESSION_REFRESH_EACH_REQUEST\": {\n      \"type\": \"boolean\",\n      \"description\": \"Refresh cookie on each request.\",\n      \"default\": true\n    },\n    \"JSON_SORT_KEYS\": {\n      \"type\": \"boolean\",\n      \"description\": \"Sort keys in JSON responses.\",\n      \"default\": true\n    },\n    \"JSONIFY_MIMETYPE\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type for jsonify responses.\",\n      \"default\": \"application/json\"\n    },\n    \"TEMPLATES_AUTO_RELOAD\": {\n      \"type\": \"boolean\",\n      \"description\": \"Auto-reload templates on change.\"\n    },\n    \"EXPLAIN_TEMPLATE_LOADING\": {\n      \"type\": \"boolean\",\n      \"description\": \"Log template loading for debugging.\",\n      \"default\": false\n    },\n    \"TRAP_HTTP_EXCEPTIONS\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trap HTTP exceptions for debugging.\",\n      \"default\": false\n    },\n    \"TRAP_BAD_REQUEST_ERRORS\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Trap bad request errors.\",\n      \"default\": false\n    },\n    \"PROPAGATE_EXCEPTIONS\": {\n      \"type\": \"boolean\",\n      \"description\": \"Propagate exceptions instead of handling.\"\n    },\n    \"SQLALCHEMY_DATABASE_URI\": {\n      \"type\": \"string\",\n      \"description\": \"SQLAlchemy database connection URI (Flask-SQLAlchemy extension).\"\n    },\n    \"SQLALCHEMY_TRACK_MODIFICATIONS\": {\n      \"type\": \"boolean\",\n      \"description\": \"Track SQLAlchemy model modifications.\",\n      \"default\": false\n    },\n    \"SQLALCHEMY_ECHO\": {\n      \"type\": \"boolean\",\n      \"description\": \"Echo SQL statements.\",\n      \"default\": false\n    },\n    \"SQLALCHEMY_POOL_SIZE\": {\n      \"type\": \"integer\",\n      \"description\": \"Connection pool size.\",\n      \"default\": 5\n    },\n    \"SQLALCHEMY_POOL_TIMEOUT\": {\n      \"type\": \"integer\",\n      \"description\": \"Pool checkout timeout in seconds.\",\n\
  \      \"default\": 10\n    },\n    \"SQLALCHEMY_MAX_OVERFLOW\": {\n      \"type\": \"integer\",\n      \"description\": \"Max connections beyond pool size.\",\n      \"default\": 10\n    },\n    \"MAIL_SERVER\": {\n      \"type\": \"string\",\n      \"description\": \"Mail server hostname (Flask-Mail extension).\",\n      \"default\": \"localhost\"\n    },\n    \"MAIL_PORT\": {\n      \"type\": \"integer\",\n      \"description\": \"Mail server port.\",\n      \"default\": 25\n    },\n    \"MAIL_USE_TLS\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use TLS for mail.\",\n      \"default\": false\n    },\n    \"MAIL_USE_SSL\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use SSL for mail.\",\n      \"default\": false\n    },\n    \"MAIL_USERNAME\": {\n      \"type\": \"string\",\n      \"description\": \"Mail server username.\"\n    },\n    \"MAIL_PASSWORD\": {\n      \"type\": \"string\",\n      \"description\": \"Mail server password.\"\n    },\n    \"CACHE_TYPE\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Cache backend type (Flask-Caching extension).\",\n      \"enum\": [\"NullCache\", \"SimpleCache\", \"FileSystemCache\", \"RedisCache\", \"MemcachedCache\"],\n      \"default\": \"NullCache\"\n    },\n    \"CACHE_DEFAULT_TIMEOUT\": {\n      \"type\": \"integer\",\n      \"description\": \"Default cache timeout in seconds.\",\n      \"default\": 300\n    },\n    \"CACHE_REDIS_URL\": {\n      \"type\": \"string\",\n      \"description\": \"Redis URL for cache backend.\"\n    },\n    \"CORS_ORIGINS\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed origins for CORS (Flask-CORS extension).\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CORS_METHODS\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed HTTP methods for CORS.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CORS_SUPPORTS_CREDENTIALS\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Allow credentials in CORS requests.\",\n      \"default\": false\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/flask/refs/heads/main/json-schema/flask-config.json
tags:
- Frameworks
- Lightweight
- Microframework
- Pallets
- Python
- Web Framework
- WSGI
title: Flask Application Configuration
---
