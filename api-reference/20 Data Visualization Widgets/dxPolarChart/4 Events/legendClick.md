---
type: eventType
---
---
##### notUsedInTheme

##### shortDescription
Fires when an item on the chart legend is clicked.

##### param(e): object
Information about the event.

##### field(e.component): object
The [widget's instance](/api-reference/10%20UI%20Widgets/Component/3%20Methods/instance().md '/Documentation/ApiReference/Data_Visualization_Widgets/dxPolarChart/Methods/#instance').

##### field(e.element): object
The widget's container.

##### field(e.jQueryEvent): jQuery-event object
The jQuery event.

##### field(e.target): series
The series to which the clicked legend item belongs.

---
When implementing a handling function, use the object passed to it as its parameter. Among the fields of this object, you can find the series to which the clicked legend item belongs. To learn about series' members you can use, refer to the description of the [Series](/api-reference/20%20Data%20Visualization%20Widgets/dxPolarChart/7%20Chart%20Elements/Series '/Documentation/ApiReference/Data_Visualization_Widgets/dxPolarChart/Chart_Elements/Series/') object.

#####See Also#####
#include common-link-handleevents