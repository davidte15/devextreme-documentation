---
id: dxFilterBuilder.Options.onEditorPrepared
type: function(e)
default: null
EventForAction: dxFilterBuilder.editorPrepared
---
---
##### shortDescription
A function that is executed after an editor is created.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The widget's [instance](/api-reference/10%20UI%20Widgets/Component/3%20Methods/instance().md '/Documentation/ApiReference/UI_Widgets/dxFilterBuilder/Methods/#instance').

##### field(e.dataField): String
The data field's name.

##### field(e.disabled): Boolean
Indicates whether the editor is disabled.

##### field(e.editorElement): dxElement
#include common-ref-elementparam with { element: "editor" }

##### field(e.editorName): String
The editor's name.

##### field(e.element): dxElement
#include common-ref-elementparam with { element: "widget" }

##### field(e.filterOperation): String
The applied filter operation.

##### field(e.model): Object
The model data. Available only if you use Knockout.

##### field(e.readOnly): Boolean
Indicates whether the editor is read-only.

##### field(e.rtlEnabled): Boolean
Indicates whether the editor uses right-to-left representation.

##### field(e.setValue(newValue)): any
A method that you need to call to change the field's value after the editor's value changes.

##### field(e.updateValueTimeout): Number
Gets and sets the delay between when a user stops typing the field's value and when it is applied.

##### field(e.value): any
The editor's value.

##### field(e.width): Number
The editor's width.

---
The widget offers a user a different editor for entering a value depending on the field's [dataType](/api-reference/10%20UI%20Widgets/dxFilterBuilder/5%20Field/dataType.md '/Documentation/ApiReference/UI_Widgets/dxFilterBuilder/Field/#dataType'): [Calendar](/concepts/05%20Widgets/Calendar/00%20Overview.md '/Documentation/Guide/Widgets/Calendar/Overview/'), [TextBox](/concepts/05%20Widgets/TextBox/00%20Overview.md '/Documentation/Guide/Widgets/TextBox/Overview/'), [SelectBox](/concepts/05%20Widgets/SelectBox/00%20Overview.md '/Documentation/Guide/Widgets/SelectBox/Overview/'), etc. You can customize automatically created editors using this function.

[note]This function is not executed for fields that use the [editorTemplate](/api-reference/10%20UI%20Widgets/dxFilterBuilder/5%20Field/editorTemplate.md '/Documentation/ApiReference/UI_Widgets/dxFilterBuilder/Field/#editorTemplate').