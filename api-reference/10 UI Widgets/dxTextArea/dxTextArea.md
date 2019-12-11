---
module: ui/text_area
export: default
inherits: ..\dxTextBox\dxTextBox.md
---
---
##### widgettree

##### lib
dx.mobile.js, dx.web.js, dx.viz-web.js, dx.all.js

##### shortDescription
The **TextArea** is a widget that enables a user to enter and edit a multi-line text.

---
You can create the widget using one of the following approaches.

---
#####[**jQuery**](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/Create_and_Configure_a_Widget/')  

    <!--JavaScript-->$(function() {
        $("#textArea").dxTextArea({
            placeholder: "Type a text here..."
        });
    });

    <!--HTML-->
    <div id="textArea"></div>

#####[**Angular**](/concepts/00%20Getting%20Started/15%20Widget%20Basics%20-%20Angular/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Angular/Create_and_Configure_a_Widget/')  

    <!--HTML-->
    <dx-text-area placeholder="Type a text here..."></dx-text-area>

#####[**AngularJS**](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/Create_and_Configure_a_Widget/')  

    <!--HTML-->
    <div dx-text-area="{
        placeholder: 'Type a text here...'
    }"></div>

#####[**Knockout**](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/Create_and_Configure_a_Widget/')  

    <!--HTML-->
    <div data-bind="dxTextArea: {
        placeholder: 'Type a text here...'
    }"></div>

#####[**ASP.NET MVC Controls**](/concepts/35%20ASP.NET%20MVC%20Controls/20%20Fundamentals/05%20Creating%20a%20Widget.md '/Documentation/Guide/ASP.NET_MVC_Controls/Fundamentals/#Creating_a_Widget')

    <!--Razor C#-->@(Html.DevExtreme().TextArea()
        .ID("textArea")
        .Placeholder("Type a text here...")
    )

    <!--Razor VB-->@(Html.DevExtreme().TextArea() _
        .ID("textArea") _
        .Placeholder("Type a text here...")
    )

---

Note that DevExtreme widgets require you to link the jQuery library to your application. If you use the Knockout or AngularJS approach, the Knockout or AngularJS library is also required. For detailed information on linking these libraries to your project, refer to the topics in the [Installation](/concepts/00%20Getting%20Started/01%20Installation/01%20Local%20Scripts.md '/Documentation/Guide/Getting_Started/Installation/Local_Scripts/') section.

#include common-demobutton with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/#demo/editorstextareatextareatextarea/"
}

#####See Also#####
- [TextArea - Overview](/concepts/05%20Widgets/TextArea/00%20Overview.md '/Documentation/Guide/Widgets/TextArea/Overview/')