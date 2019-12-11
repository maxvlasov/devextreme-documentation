---
type: eventType
---
---
##### notUsedInTheme

##### shortDescription
Fires when a point's tooltip becomes hidden.

##### param(e): object
Information about the event.

##### field(e.component): object
The [widget's instance](/api-reference/10%20UI%20Widgets/Component/3%20Methods/instance().md '{basewidgetpath}/Methods/#instance').

##### field(e.element): object
The widget's container.

##### field(e.target): Point
The series point whose tooltip becomes hidden.

---
The point's tooltip becomes invisible when a user hovers the mouse cursor over another series point. In addition, you can hide a tooltip in code, using the **hideTooltip()** method of the chart or point.

When a tooltip is made hidden, you can perform specific actions by handling the **tooltipHidden** event. When implementing a handling function, use the object passed to it as its parameter. Among the fields of this object, you can find the series point whose tooltip becomes hidden.

#####See Also#####
#include common-link-handleevents