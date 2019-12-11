---
type: eventType
---
---
##### notUsedInTheme

##### shortDescription
Fires when the user clicks a node.

##### param(e): object
Information about the event.

##### field(e.component): object
The widget's instance.

##### field(e.element): object
The widget's container.

##### field(e.jQueryEvent): jQuery-event object
The jQuery event.

##### field(e.node): dxtreemapnode
The clicked node.

---
When implementing a handling function, use the object passed to it as the parameter. Among the fields of this object, you can find the clicked node. To learn about node's members that you can use, refer to the description of the [Node](/api-reference/20%20Data%20Visualization%20Widgets/dxTreeMap/6%20Node '/Documentation/ApiReference/Data_Visualization_Widgets/dxTreeMap/Node/') object.

To handle this event, attach a handler to it using the [on(eventName, eventHandler)](/api-reference/10%20UI%20Widgets/EventsMixin/3%20Methods/on(eventName_eventHandler).md '/Documentation/ApiReference/Data_Visualization_Widgets/dxTreeMap/Methods/#oneventName_eventHandler') method. For example, the handler in the following code selects/deselects the clicked node.

    <!--JavaScript-->// ...
    var selectNode = function (e) {
        e.node.select(!e.node.isSelected());
    };
    
    treeMapInstance.on('click', selectNode);
    
#####See Also#####
#include common-link-handleevents