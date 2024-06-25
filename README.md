<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/523321257/22.1.4%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T1108986)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
[![](https://img.shields.io/badge/💬_Leave_Feedback-feecdd?style=flat-square)](#does-this-example-address-your-development-requirementsobjectives)
<!-- default badges end -->

# Blazor Grid - Create a ComboBox (Foreign Key) Column

A foreign key is a database key used to manage relations between tables. You can use it to identify a specific row in the referenced table and obtain row data. You can use following two techniques to display this relationship within the DevExpress Blazor Grid component:

![Grid with ComboBox column](result.png)

First option, you can create a [dictionary](./CS/GridForeignColumn/Pages/Index.razor#L65) that contains the category's ID and name. Use this dictionary to obtain [display text](./CS/GridForeignColumn/Pages/Index.razor#L85) in the [CustomizeCellDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.CustomizeCellDisplayText) event handler for the **Category Name** column.

Alternatively, the **Category Name** column can remain unbound. [Specify](./CS/GridForeignColumn/Pages/UnboundColumn.razor#L60) the column's cell value in the [UnboundColumnData](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.UnboundColumnData) event handler.

In both instances, you can create a [data column cell editor](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.DataColumnCellEditTemplate) or [cell editor](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.CellEditTemplate) template and place a [combo box](./CS/GridForeignColumn/Pages/Index.razor#L38) in it (this will allow users to select the appropriate value for the **Category Name** column).

## Files to Review

- [Index.razor](./CS/GridForeignColumn/Pages/Index.razor)
- [UnboundColumn.razor](./CS/GridForeignColumn/Pages/UnboundColumn.razor)

## Documentation

- [DataColumnCellEditTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.DataColumnCellEditTemplate)
- [CustomizeCellDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.CustomizeCellDisplayText)
- [UnboundColumnData](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.UnboundColumnData)

## More Examples

- [Blazor Grid - Post changes to an in-memory data source](https://github.com/DevExpress-Examples/blazor-dxgrid-instantly-update-data-item-fields)
<!-- feedback -->
## Does this example address your development requirements/objectives?

[<img src="https://www.devexpress.com/support/examples/i/yes-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=blazor-grid-foreignkey-column&~~~was_helpful=yes) [<img src="https://www.devexpress.com/support/examples/i/no-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=blazor-grid-foreignkey-column&~~~was_helpful=no)

(you will be redirected to DevExpress.com to submit your response)
<!-- feedback end -->
