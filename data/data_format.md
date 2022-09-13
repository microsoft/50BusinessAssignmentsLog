
# Data Format for Recording of Business Tasks
## Introduction
Dataset Name: Recordings of 50 business assignments.

Many business applications are used to help carry out business processes effectively. These application range from email clients, web browsers, document editors and many other productivity tools. 

The aim of this dataset is to present various scenarios of day to day work which can be automated.

The dataset is composed of 50 processess, with 3 recordings in each process. 


## List of columns: 
The format of the data includes the following columns: 
- StepId
- RecordingId
- ProcessId
- TimeStamp
- StepName
- StepDescription
- ApplicationProcessName
- ApplicationParentWindowName
- AutomationStep
- NextStepId
- label_EventName
- label_EventId

## Description of the Columns 
Columns in the dataset include:

Column Name | Description
------ | ------ 
StepId          | The number of the step within the recording. 
RecordingId     | ID of the recording.
ProcessId       | ID of the process, for which the recording was done. 
TimeStamp       | Timestamp of the step within the recoridng. 
StepName        | Name of the step. It is one of 19 different options, please see below for details. 
StepDescription         | More detailed description of the step. 
ApplicationProcessName  | Process Name, taken from the opened application.
ApplicationParentWindowName |  Parent Window Name, taken from the opened application.
AutomationCode         | A Script which could be used to automate that step. 
label_EventName         | Event name given by a person making the recording for the groupped steps. 
label_EventId           | ID of the group of steps, called an Event. 
------ 


# Column Details
## StepId
ID of the step within the recording of the process.


## RecordingId
ID of the recording within the process.  Every process is typically recorded 3 times.


## ProcessId
ID of the process. The process is defined on a high level by up to 3 tasks which needs to be achieved. This tasks use various business applications, detailed in the ApplicationParentWindowName.

## TimeStamp
Time when the specific step was recorded. 


## StepName
Step Name is a standardized name of the action taken by the user. It is one of the 19 values below, with the following distribution:
StepName | Count
----- | -----
Click UI element in window | 2504
Press button in window | 1406
Populate text field in window | 718
Select menu option in window | 404
Send keys | 387
Drag and drop UI element in window | 110
Select tab in window | 75
Set checkbox state in window | 44
Set drop-down list value in window | 20
Select radio button in window | 16
MouseAndKeyboard.SendKeys.FocusAndSendKeys | 15
Expand/collapse tree node in window | 9
Comment | 2
Move window | 2
Prepare a form for employees feedback | 0
Close window | 1
Resize window | 1
Locate the Notification and review it in Inbox of mailing app | 1
Get details of a UI element in window | 1



## StepDescription
Extended description of each step. 

## ApplicationProcessName
Name of the process associated with the application. 

## ApplicationParentWindowName
Table below presents the number of steps which are done within a specific application.
ApplicationProcessName | Count of steps
----- | -----
chrome | 1661
msedge | 1128
firefox | 884
Teams | 570
PBIDesktop | 125
OUTLOOK | 119
ApplicationFrameHost | 107
Ssms | 46
CoollePDFConverter | 42
SearchApp | 38
OneDrive | 27
ONENOTE | 26
explorer | 21
Skype | 19
EXCEL | 16
ShellExperienceHost | 13
cmd | 3


## AutomationCode
Code which can be used for automating the step.


## NextStepId
ID of the next step. This Id corresponds to StepID field.


## label_EventName
Human label for EventName, which groups certain tasks together into an event. 

##  label_EventId
Human label for ID for the Event.
