---
description: "Automatically generated file. DO NOT MODIFY"
---

```cli

mgc security triggers retention-events create --body '{\
  "@odata.type": "#microsoft.graph.security.retentionEvent",\
  "displayName": "String",\
  "description": "String",\
  "eventQuery": [\
    {\
      "@odata.type": "microsoft.graph.security.eventQuery"\
    }\
  ],\
  "eventTriggerDateTime": "String (timestamp)",\
  "createdBy": {\
    "@odata.type": "microsoft.graph.identitySet"\
  },\
  "eventPropagationResults": [\
    {\
      "@odata.type": "microsoft.graph.security.eventPropagationResult"\
    }\
  ],\
  "eventStatus": {\
    "@odata.type": "microsoft.graph.security.retentionEventStatus"\
  },\
  "lastStatusUpdateDateTime": "String (timestamp)"\
}\
'

```