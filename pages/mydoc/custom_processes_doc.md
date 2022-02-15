---
title: Custom processes description
keywords: processes
last_updated: July 3, 2022
tags: [workflows processes]
summary: "The description of custom processes"
sidebar: mydoc_sidebar
permalink: custom_processes_doc.html
folder: mydoc
---

## Summary

The custom process is predefined by user automation linked to a resource (AWS lambda function). Every workflow can consist of any amount of custom processes.

The custom process has input and output properties. For example, there is a "send email" process. The input properties will be:
- email
- subject
- message

The output property will be:
- success

Whenever workflow launches a process, it triggers a corresponding AWS lambda function and passes input data from the workflow's state. Lambda function then gets executed and returns a response to the workflow.

## Creating a new custom process

You have to go to the new process page to create a new custom process.

{% include image.html file="new_process.gif" url="http://jekyllrb.com" alt="New process" caption="New process" %}
