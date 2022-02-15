---
title: Embeddable workflows
keywords: api
last_updated: July 3, 2022
tags: [api]
summary: "This is an insturction how to generate en embeddable workflow link"
sidebar: mydoc_sidebar
permalink: embeddable_workflows_doc.html
folder: mydoc
---

## Summary

The embeddable workflow editor is designed to be embedded into your software to allow your customers to create automations in the scope of your solution.

## Preparation

To generate an embeddable workflow, you need to have an access token that you can generate inside the Adminix dashboard. You should also create a workflow via API to get a workflow ID.

## Generating a link

```
curl -XPOST -H 'Authorization: Bearer <your-access-token>' -H "Content-type: application/json" 'https://api.adminix.xyz/api/v1/workflows/<your-workflow-id>/generate_embeddable_link'
```

Please replace <your-access-token> with your access token and <your-workflow-id> with your workflow ID.
