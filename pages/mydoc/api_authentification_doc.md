---
title: API authentification
keywords: api
last_updated: July 3, 2022
tags: [api]
summary: "This is an API authentification documentation page"
sidebar: mydoc_sidebar
permalink: api_authentification.html
folder: mydoc
---

## Creating access token

To create API access credentials, you need to go to [Profile settings](https://app.adminix.xyz/profile/edit). Scroll down to the "Personal access tokens" section and generate a new token.

{% include image.html file="new_access_token.gif" alt="New access token" caption="New access token" %}

## Sending authentificated API request

To send authenticated API request, you need to provide an Authorization header in the request.

```
Authorization: Bearer <your-access_token>
```

## Example request to get a current session

```
curl -XGET -H 'Authorization: Bearer <your-access_token>' -H "Content-type: application/json" 'https://api.adminix.xyz/api/v1/auth/me'
```
