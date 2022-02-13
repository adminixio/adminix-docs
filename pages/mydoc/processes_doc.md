---
title: Processes description
keywords: processes
last_updated: July 3, 2022
tags: [workflows processes]
summary: "The provider is a connection between Adminix and AWS account"
sidebar: mydoc_sidebar
permalink: processes_doc.html
folder: mydoc
---

Each workflow consists of a chain of processes. The process is a business logic that runs a code responsible for doing some logic. Every process has input and output properties.

There are default and custom processes. The default processes are predefined by Adminix workflow and can't be customized. The custom processes can be configured inside the processes management page.

There are seven default processes:
{% include image.html file="processes.png" url="http://jekyllrb.com" alt="Jekyll" caption="This is a sample caption" %}

The end node should be placed at the end of the chain. Every workflow should have at least one end node. The end node can have a status of success or failure.

The condition defines a start of condition branching logic. It has a title that can be customized.

The case defines a new branch of the condition. The condition can have multiple cases. Each case has rules. The rule is a logical condition.

Else defines the else condition. Each condition can have only one else node. The else node doesn't have rules in it.

The delay node is responsible for delaying the workflow for some period of time. It has
