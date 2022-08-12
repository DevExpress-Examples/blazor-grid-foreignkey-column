<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/523321257/22.1.4%2B)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->

# Blazor Grid - Create a ComboBox (Foreign Key) Column

A foreign key is a database key that is used to show relations between tables. You can use it to identify a particular row in the referenced table and obtain data of this row. The Grid component allows you to display this kind of data relation. You can use two approaches to achieve this.

![Grid with ComboBox column](result.png)

In the first approach, create a [dictionary](./CS/GridForeignColumn/Pages/Index.razor#L65) that contains category's ID and name. Use this dictionary to obtain the [display text](./CS/GridForeignColumn/Pages/Index.razor#L85) in the [CustomizeCellDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.CustomizeCellDisplayText) event handler for the **Category Name** column.

In the second approach, the **Category Name** column is unbound. [Specify](./CS/GridForeignColumn/Pages/UnboundColumn.razor#L60) the column's cell values in the [UnboundColumnData](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.UnboundColumnData) event handler.

In both variants, create a [DataColumnCellEditTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.DataColumnCellEditTemplate) or [CellEditTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.CellEditTemplate) and place there a [ComboBox](./CS/GridForeignColumn/Pages/Index.razor#L38) that allows users to choose the **Category Name** value.

## Files to Look At

- [Index.razor](./CS/GridForeignColumn/Pages/Index.razor)
- [UnboundColumn.razor](./CS/GridForeignColumn/Pages/UnboundColumn.razor)

## Documentation

- [DataColumnCellEditTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.DataColumnCellEditTemplate)
- [CustomizeCellDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.CustomizeCellDisplayText)
- [UnboundColumnData](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.UnboundColumnData)

## More Examples

- [Blazor Grid - Post changes to an in-memory data source](https://github.com/DevExpress-Examples/blazor-dxgrid-instantly-update-data-item-fields)
