---
title: Creating a new provider
keywords: documentation theme, jekyll, technical writers, help authoring tools, hat replacements
last_updated: July 3, 2022
tags: [providers]
summary: "The provider is a connection between Adminix and AWS account"
sidebar: mydoc_sidebar
permalink: new_provider_doc.html
folder: mydoc
---

1. To create a resource, you have to go to the resources page by clicking on the resources link in the left menu.
   {% include image.html file="resources_button.png" url="http://jekyllrb.com" alt="Jekyll" caption="This is a sample caption" %}
2. Then you need to click on the "Add" button
   {% include image.html file="new_resource_button.png" url="http://jekyllrb.com" alt="Jekyll" caption="This is a sample caption" %}
2. Fill up the form and click "save"
   - The resource type is the type of AWS resource. For now, it can only be the "Lambda function."
   - The name is a name of this resource you will see in the list
   - The description input is an optional value to describe additional details about this resource
   - The function name is the current AWS lambda function name
   - The function version is the latest version of the AWS function
   - Please enable the async option if you want this resource to be async. It means that workflow can wait until this resource finishes his job.
   - Please provide resource properties. These are input properties of the resource which than passed to a lambda function

   {% include image.html file="new_resource_page.png" url="http://jekyllrb.com" alt="Jekyll" caption="This is a sample caption" %}
   
