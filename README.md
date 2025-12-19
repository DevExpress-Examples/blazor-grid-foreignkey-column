<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/523321257/25.1.3%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T1108986)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
[![](https://img.shields.io/badge/💬_Leave_Feedback-feecdd?style=flat-square)](#does-this-example-address-your-development-requirementsobjectives)
<!-- default badges end -->

# Blazor Grid - Create a ComboBox (Foreign Key) Column

As you know, a foreign key is a database key used to manage relationships between individual tables. You can use the key to identify a specific column in a referenced table (and obtain column data). This example illustrates the use of foreign keys within the [DevExpress Blazor Grid](https://docs.devexpress.com/Blazor/403143/components/grid) UI component.

![Grid with ComboBox column](result.png)

To create a foreign key column in the DevExpress Blazor Grid component, you must:
1.	Add a [DxGridDataColumn](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn) object to the Grid's column collection.
2.	Assign the field name that stores foreign keys to the column's [FieldName](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.FieldName) property.
3.	Place [DxComboBoxSettings](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxComboBoxSettings) within the column's [EditSettings](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridDataColumn.EditSettings) tag.
4.	Assign an external data source to the [Data](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxComboBoxSettings.Data) combo box setting.
5.	Assign the name of the external data source field that stores foreign keys to the [ValueFieldName](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxComboBoxSettings.ValueFieldName) setting. The [TextFieldName](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxComboBoxSettings.TextFieldName) setting allows you specify text strings displayed within the Grid (instead of foreign keys).

## Files to Review

- [Index.razor](./CS/GridForeignColumn/Pages/Index.razor)

## Documentation

* [Edit Data](https://docs.devexpress.com/Blazor/403454/components/grid/edit-data)

## More Examples

- [Blazor Grid - Post changes to an in-memory data source](https://github.com/DevExpress-Examples/blazor-dxgrid-instantly-update-data-item-fields)
<!-- feedback -->
## Does this example address your development requirements/objectives?

[<img src="https://www.devexpress.com/support/examples/i/yes-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=blazor-grid-foreignkey-column&~~~was_helpful=yes) [<img src="https://www.devexpress.com/support/examples/i/no-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=blazor-grid-foreignkey-column&~~~was_helpful=no)

(you will be redirected to DevExpress.com to submit your response)
<!-- feedback end -->
