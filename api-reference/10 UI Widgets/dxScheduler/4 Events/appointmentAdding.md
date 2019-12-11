---
type: eventType
---
---
##### shortDescription
Fires before an appointment is added to the data source.

##### param(e): object
Information about the event.

##### field(e.component): object
The widget [instance](/api-reference/10%20UI%20Widgets/Component/3%20Methods/instance().md '/Documentation/ApiReference/UI_Widgets/dxScheduler/Methods/#instance').

##### field(e.element): jQuery
The widget's container.

##### field(e.model): object
Data that is available for binding against the element. Available only in the Knockout approach.

##### field(e.appointmentData): Object
The appointment object to be added to the data source.

##### field(e.cancel): Boolean|Promise
A flag allowing you to prevent the appointment from being added to the data source.

---
Instead, you can use the [onAppointmentAdding](/api-reference/10%20UI%20Widgets/dxScheduler/1%20Configuration/onAppointmentAdding.md '/Documentation/ApiReference/UI_Widgets/dxScheduler/Configuration/#onAppointmentAdding') option to handle the event.

#####See Also#####
#include common-link-handleevents