---
title: Personal information tokenization and storage
summary: Databunker provides built-in support for PII tokenization and storage.
abstract: ""
weight: 10
authors: []
tags: []
featured: false

image:
  caption: 'Image'
  focal_point: Right

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
# - internal-project

# Enable math on this page?
math: true
---

{{% alert note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /alert %}}

Databunker is basically special encrypted database for customer information, or PII in terms of GDPR.

Upon a special API request to create a new user records is received, on request parameters provided as HTML POST key/value format or as JSON format, Databunker performs the following operations:

- Request sanity check and access token check.
- Normalize email address, phone number, login name.
- Strict user shema check if schema is defined in configuration and return error if something is missing.
- Encrypt email address, phone number, login name.
- Validate for duplicate records using encrypted keys (email, phone, login) and return user exists error.
- Generate a record UUID to be used as a user token.
- Encrypt the whole user record and save it in backend database already encrypted (MySQL, PostgreSQL, SQLite)
- Return user token (UUID generated previously).

Now, when Databunker returns you customer token, you can use it with your existing database instead of stroing personal records.

Afterwords, you can query the Databunker service to receive personal information, saving audit trail.