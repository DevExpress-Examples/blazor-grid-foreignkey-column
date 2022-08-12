<!-- default badges list -->
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->

# Blazor Grid - Create a ComboBox (Foreign Key) Column

A foreign key is a database key used to show relations between tables. You can use it to identify a particular row in the referenced table and obtain data from this row. You can use following two techniques to display this relation in the Grid component:

![Grid with ComboBox column](result.png)

As the first option, you can create a [dictionary](./CS/GridForeignColumn/Pages/Index.razor#L65) that contains the category's ID and name. Use this dictionary to obtain [display text](./CS/GridForeignColumn/Pages/Index.razor#L85) in the [CustomizeCellDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.CustomizeCellDisplayText) event handler for the **Category Name** column.

Alternatively, the **Category Name** column can be unbound. [Specify](./CS/GridForeignColumn/Pages/UnboundColumn.razor#L60) the column's cell values in the [UnboundColumnData](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.UnboundColumnData) event handler.

In both cases, you can create a [data column cell editor](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.DataColumnCellEditTemplate) or [cell editor](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.CellEditTemplate) template and place a [combo box](./CS/GridForeignColumn/Pages/Index.razor#L38) in it to allow users to choose the **Category Name** value.

## Files to Look At

- [Index.razor](./CS/GridForeignColumn/Pages/Index.razor)
- [UnboundColumn.razor](./CS/GridForeignColumn/Pages/UnboundColumn.razor)

## Documentation

- [DataColumnCellEditTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.DataColumnCellEditTemplate)
- [CustomizeCellDisplayText](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.CustomizeCellDisplayText)
- [UnboundColumnData](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGrid.UnboundColumnData)

## More Examples

- [Blazor Grid - Post changes to an in-memory data source](https://github.com/DevExpress-Examples/blazor-dxgrid-instantly-update-data-item-fields)
