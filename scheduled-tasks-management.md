---
title: Scheduled Tasks Management
page_title: Scheduled Tasks Management
description: Scheduled Tasks Management
slug: tasks-management
tags: scheduling,tasks,management
published: True
position: 700
---

# Scheduled Tasks Management



The **Scheduling** view is a centralized place from which you can manage scheduled tasks, review the created by the tasks documents and manage subscribers.

Scheduling
----------

The **Scheduling** view allows you to create, modify and delete scheduled tasks. A scheduled task specifies when a specific report should be rendered and in what document format. The created documents are stored in the Report Server's storage and can be sent as email attachments to different subscribers. A scheduled task can be run only once or on a recurrent basis, for example: daily, weekly, monthly or yearly. Within the recurrence rule, you set the intervals and range for how often a report execution is to occur.

A task has the following settings:

-   **Name** - the name of the task. It should be unique among the tasks

-   A report represented by its Category and Name

-   Target document format - can be any single document format provided by the Telerik Reporting engine:

    -   PDF - Renders a report in the Adobe Acrobat Reader. The format is shown as Acrobat (PDF) File in the Export drop-down of the report toolbar.

    -   XLS - Renders a report in Microsoft Excel. The report opens in Microsoft Excel 97 or later.

    -   CSV - Renders a report in comma-delimited format. The report opens in a viewing tool associated with CSV file formats.

    -   RTF - Renders a report in Rich Text Format. The report opens in Microsoft Word 97 or later.

    -   XPS - Renders a report in XML Paper Specification (XPS) format - electronic representation of digital documents based on XML. The report opens in Microsoft XPS Viewer.

    -   DOCX - Renders a report in Microsoft Word 2007 format (also known as OpenXML) - it is a zipped, XML-based file format developed by Microsoft for representing word processing documents.

    -   XLSX - Renders a report in Microsoft Excel 2007 format (also known as OpenXML) - it is a zipped, XML-based file format developed by Microsoft for representing spreadsheets.

    -   PPTX - Renders a report in Microsoft PowerPoint 2007 format (also known as OpenXML) - it is a zipped, XML-based file format developed by Microsoft for presentations.

    -   MHTML - Renders a report in MHTML. The report opens in Internet Explorer. The format is shown as Web Archive in the Export drop-down of the report toolbar.

-   **Enabled** - the task can be temporary disabled without the need to delete it

-   **Start** - the actual start date of the task

-   **Repeat** - defines the recurrence rule if the task should be executed on regular intervals. The repeat pattern can be daily, weekly, monthly and yearly. Currently, hourly repetition is not supported.

-   **Parameters** - the task parameters allow you to define the parameter values that will be used for the report when the task is executed. The parameters area includes all report parameters of the report regardless their visibility (visible or invisible). By default the invisible report parameters will use their values specified at design time, i.e. they are not overridden by the parameter values specified in the task. If you want to override the invisible parameters' values with the task's parameters you have to uncheck the "*Use Default Value*" checkbox.
The "*Use Default Value*" checkbox for all parameters determines whether the value of the report parameter specified at design time will be used or whether it will be overridden by the value that you have specified in the task's parameters. When it is checked the design time value of the report parameter will be used and when it is unchecked the stored in the task parameters value will be used.

A new task can be also created directly from the **Reports** | **Scheduling** view.

You can search for tasks by their Name, Report, or Document Format. For more information, see [Search]({%slug search%}).

Activity view
-------------

The **Activity** view for a scheduled task shows the created by the task documents. A created document can be downloaded for preview in the target format or deleted. The list items also display whether the task has successfully created a document or there was an error while generating it.

Subscribers view
----------------

From the **Subscribers** view, you can manage who will receive the created documents as mail attachments. A subscriber can be an existing report server user or an external user which is represented through his email. The external emails should be separated with semicolon (;) or comma (,).
