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
{% include image.html file="processes.png" max-width="200" alt="Default processes" caption="Adminix default processes" %}

The end node should be placed at the end of the chain. Every workflow should have at least one end node. The end node can have a status of success or failure.

{% include image.html file="end_process.png" max-width="400" alt="Jekyll" caption="The end process" %}

The condition defines a start of condition branching logic. It has a title that can be customized.

{% include image.html file="condition_process.png" max-width="400" alt="Condtion" caption="The condition process" %}

The case defines a new branch of the condition. The condition can have multiple cases. Each case has rules. The rule is a logical condition.

{% include image.html file="case_process.png" max-width="400" alt="Case" caption="The case process" %}

Else defines the else condition. Each condition can have only one else node. The else node doesn't have rules in it.

{% include image.html file="else_process.png" max-width="400" alt="Else" caption="The else process" %}

The delay node is responsible for delaying the workflow for some period of time. It has

{% include image.html file="delay_process.png" max-width="400" alt="Delay" caption="The delay process" %}

The set parameters node is responsible for setting additional data into the state of the workflow. You can specify multiple values in one node. Each value can have a different type.

{% include image.html file="set_parameter_process.png" max-width="400" alt="Set parameters" caption="The set parameters process" %}

The call workflow node is responsible for calling external workflow inside the existing one.

{% include image.html file="call_workflow_process.png" max-width="400" alt="Call workflow" caption="The call workflow process" %}
