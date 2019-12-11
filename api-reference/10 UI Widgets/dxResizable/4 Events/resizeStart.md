---
type: eventType
---
---
##### shortDescription
Fires when an end user started to resize the widget.

##### param(e): object
Provides function parameters.

##### field(e.component): object
Provides access to the widget's instance.

##### field(e.element): jQuery
An HTML element of the widget.

##### field(e.model): object
Provides access to the data that is available for binding against the element. Available only in the Knockout approach.

##### field(e.jQueryEvent): jQueryEvent
Specifies the jQuery event that caused action execution.

##### field(e.width): number
The current widget width.

##### field(e.height): number
The current widget height.

---
Instead, you can use the [onResizeStart](/api-reference/10%20UI%20Widgets/dxResizable/1%20Configuration/onResizeStart.md '/Documentation/ApiReference/UI_Widgets/dxResizable/Configuration/#onResizeStart') option to handle the event.

#####See Also#####
#include common-link-handleevents