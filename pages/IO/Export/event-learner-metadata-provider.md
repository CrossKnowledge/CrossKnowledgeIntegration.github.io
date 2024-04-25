---
title: Event Learner Metadata
keywords:
last_updated: September, 2019
tags:
summary: "This provider exports data related to learners in classroom events."
sidebar: home_sidebar
permalink: event-learner-metadata-provider.html
folder: Export
dynamic_content: true
columns: [candidateId, candidateGuid, candidateRefNumber, candidateName, candidateFirstname, candidateLogin, candidateEmail,
    candidateEntityAncestors, candidateEntityId, eventTitle, eventDescription, eventStartDate, eventEndDate, eventDuration,
    eventAllDay, eventVirtualRoomLink, eventTeacher, eventStatus, eventClassRoomTitle, eventClassRoomDescription,
    eventClassRoomCapacity, eventClassRoomType]
parameters: [eventClassRoomTypeFilter, eventDurationAllDayFilter, eventStatusFilter, entityIds, dateFormat,
    dateTimeFormat, templates, stripHTML, maxLength]
---

### Examples
```xml
<providers>
    <eventLearnerMetadataProvider>
        <columns>
            <candidateId/>
            <candidateGuid/>
            <candidateRefNumber/>
            <candidateName/>
            <candidateFirstname/>
            <candidateLogin/>
            <candidateEmail/>
            <candidateEntityAncestors/>
            <candidateEntityId/>
            <eventTitle/>
            <eventDescription/>
            <eventStartDate/>
            <eventEndDate/>
            <eventDuration/>
            <eventAllDay/>
            <eventVirtualRoomLink/>
            <eventTeacher/>
            <eventStatus/>
            <eventClassRoomTitle/>
            <eventClassRoomDescription/>
            <eventClassRoomCapacity/>
            <eventClassRoomType/>
        </columns>
        <parameters>
            <eventDurationAllDayFilter>Y</eventDurationAllDayFilter>
        </parameters>
    </eventLearnerMetadataProvider>
</providers>
```