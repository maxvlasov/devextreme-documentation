**DateBox** widgets are often coupled for selecting a date interval. In this case, you need to synchronize the **DateBoxes** to prevent a user from selecting an interval whose start date is later than the end date. For this, limit one **DateBox**'s range depending on the other's value as shown in the example below.

---
##### jQuery

    <!--JavaScript-->$(function() {
        var startDate = $("#startDate").dxDateBox({
            value: new Date(),
            onValueChanged: function (e) {
                endDate.option("min", e.value);
            }
        }).dxDateBox("instance");
        var endDate = $("#endDate").dxDateBox({
            value: new Date(),
            onValueChanged: function (e) {
                startDate.option("max", e.value);
            }
        }).dxDateBox("instance");
    });

    <!--HTML--><div id="startDate"></div>
    <div id="endDate"></div>

##### Angular

    <!--HTML--><dx-date-box 
        [(max)]="endValue"
        [(value)]="startValue">
    </dx-date-box>
    <dx-date-box 
        [(min)]="startValue"
        [(value)]="endValue">
    </dx-date-box>

    <!--TypeScript-->
    import { DxDateBoxModule } from 'devextreme-angular';
    // ...
    export class AppComponent {
        startValue: Date = new Date();
        endValue: Date = new Date();
    }
    @NgModule({
        imports: [
            // ...
            DxDateBoxModule
        ],
        // ...
    })

##### AngularJS

    <!--HTML--><div dx-date-box="{
        bindingOptions: {
            max: 'endValue'
            value: 'startValue'
        }
    }"></div>
    <div dx-date-box="{
        bindingOptions: {
            min: 'startValue'
            value: 'endValue'
        }
    }"></div>

    <!--JavaScript-->function Controller($scope) {
        $scope.startValue = new Date();
        $scope.endValue = new Date();
    }

##### Knockout

    <!--HTML--><div data-bind="dxDateBox: {
        max: endValue
        value: startValue
    }"></div>
    <div data-bind="dxDateBox: {
        min: startValue
        value: endValue
    }"></div>

    <!--JavaScript-->var viewModel = {
        startDate: ko.observable(new Date()),
        endDate: ko.observable(new Date()),
    };
    ko.applyBindings(viewModel);

---

Do not forget to call the [getDate()](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Date/getDate) method on the **DateBox** values when calculating the interval duration.

#####See Also#####
- **Widget Basics**: [jQuery](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/') | [Angular](/concepts/00%20Getting%20Started/15%20Widget%20Basics%20-%20Angular '/Documentation/Guide/Getting_Started/Widget_Basics_-_Angular/') | [AngularJS](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/') | [Knockout](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/')
- [DateBox - Specify Value Range](/concepts/05%20Widgets/DateBox/15%20Specify%20Value%20Range.md '/Documentation/Guide/Widgets/DateBox/Specify_Value_Range')
- [DateBox - Handle the Value Change Event](/concepts/05%20Widgets/DateBox/10%20Handle%20the%20Value%20Change%20Event.md '/Documentation/Guide/Widgets/DateBox/Handle_the_Value_Change_Event')
- [DateBox API Reference](/api-reference/10%20UI%20Widgets/dxDateBox '/Documentation/ApiReference/UI_Widgets/dxDateBox/')

[tags]date box, dateBox, editor, scheduling, overview, validate date interval