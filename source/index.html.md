---
title: API Reference

language_tabs:
  - shell

toc_footers:
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

Unfurld is a microservice that unfurls links, like Slack. It exposes a [single endpoint](#unfurl-links).

# Authentication

Unfurld is intended to be deployed behind a firewall, and hence does not support authentication as of now.

# Unfurl links

```shell
curl -XPOST "http://unfurld.herokuapp.com/api/v1/unfurl.json"
```

> The above command returns JSON structured like this:

```json
{"status": 200}
```

This endpoint extracts links from the provided content and unfurls them.

### HTTP Request

`POST http://unfurld.herokuapp.com/api/v1/unfurl.json`

### Request Body

Parameter | Mandatory | Description
--------- | --------- | -----------
content   | true      | The content to extract links from
