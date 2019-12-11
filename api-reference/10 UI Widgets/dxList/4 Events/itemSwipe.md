---
type: eventType
---
---
##### shortDescription
Fires when an item is swiped.

##### param(e): object
Provides function parameters.

##### field(e.component): object
Provides access to the widget's instance.

##### field(e.element): jQuery
An HTML element of the widget.

##### field(e.model): object
Provides access to the data that is available for binding against the element. Available only in the Knockout approach.

##### field(e.jQueryEvent): jQueryEvent
Returns an object representing the item.

##### field(e.itemData): object
The data that is bound to the swiped item.

##### field(e.itemElement): jQuery
An HTML element of the item.

##### field(e.itemIndex): number | object
The index of the swiped items. In a grouped list, the index represents an object defining the group and item indexes: { group: 0, item: 0 }.

##### field(e.direction): string
Specifies whether the swipe operation is performed in the left or right direction.

---
Instead, you can use the [onItemSwipe](/api-reference/10%20UI%20Widgets/dxList/1%20Configuration/onItemSwipe.md '/Documentation/ApiReference/UI_Widgets/dxList/Configuration/#onItemSwipe') option to handle the event.

#####See Also#####
- [List - Touch-Screen Gestures](/concepts/05%20Widgets/List/45%20End-User%20Interaction/01%20Touch-Screen%20Gestures.md '/Documentation/Guide/Widgets/List/End-User_Interaction/Touch-Screen_Gestures/')
#include common-link-handleevents