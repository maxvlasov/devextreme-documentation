---
default: 'onlyPoint'
acceptValues: 'onlyPoint' | 'allSeriesPoints' | 'allArgumentPoints' | 'none'
type: String
---
---
##### shortDescription
Specifies series elements to be highlighted when a user points to the series.

---
When a user points to the series, it may react in one of the following ways depending on the value of the **hoverMode** option.

* **onlyPoint**   
Only the series point that a user pauses on changes its style.
* **allSeriesPoints**   
All points in the series change their style.
* **allArgumentPoints**   
The series point that a user pauses on changes its style. Points with the same argument do it as well.
* **none**   
The series does not react to pointing to it.

When using the widget as an [ASP.NET MVC Control](/concepts/35%20ASP.NET%20MVC%20Controls/20%20Fundamentals '/Documentation/Guide/ASP.NET_MVC_Controls/Fundamentals/'), specify this option using the `ChartSeriesHoverMode` enum with one of the following values: `OnlyPoint`, `AllSeriesPoints`, `AllArgumentPoints`, and `None`. Note that although this enum accepts more values, only the listed ones can be applied to a stacked bar series.

#####See Also#####
- [hoverStyle](/api-reference/20%20Data%20Visualization%20Widgets/dxPolarChart/5%20Series%20Types/CommonPolarChartSeries/hoverStyle '/Documentation/ApiReference/Data_Visualization_Widgets/dxPolarChart/Series_Types/StackedBarSeries/hoverStyle/')