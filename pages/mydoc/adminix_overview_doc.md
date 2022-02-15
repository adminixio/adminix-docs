---
title: Adminix overview
keywords: api
last_updated: July 3, 2022
tags: [getting_started]
summary: "This is an Adminix overview page"
sidebar: mydoc_sidebar
permalink: adminix_overview_doc.html
folder: mydoc
---

## Introduction

Adminix is a cloud workflow automation platform designed to help companies with a digital transformation of their business processes using serverless technology.

## How Adminix works

Adminix is a SaaS platform in mind. Adminix doesn't run processes or store your private data in its cloud. Instead, all automations created by Adminix exist inside the client's AWS account. So Adminix is a platform that connects to the client's AWS account to create and run automations. Every automation created by Adminix exists inside the AWS step functions service that runs a chain of AWS lambda functions.

{% include image.html file="adminix_aws_schema.png" alt="Adminix <> AWS schema" caption="Adminix <> AWS schema" %}
