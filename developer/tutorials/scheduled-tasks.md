---
title: Scheduled Tasks
author: AndreiMaz
uid: developer/tutorials/scheduled-tasks
---
# Scheduled Tasks

With Scheduled tasks, you can schedule a task to run at certain periods. For example, nopCommerce sends queued emails periodically. The basic steps to create a new task are:

1. Define a class which implements **IScheduleTask** interface. It has only one method that takes no arguments; **Execute**. As you guessed this method is invoked when the task should be run.

1. To schedule a task the developer should insert a new **ScheduleTask** record into the appropriate database table. You can use **IScheduleTaskService** for inserting such a record.
3. When insert the new record into **ScheduleTask** database table for new **ScheduleTask**, it is important to keep **Type** column  format **Namespace.TaskClassName, AssemblyName**.



## Troubleshooting
* Make sure your store url.
* Restart the application after adding new schecule task.


