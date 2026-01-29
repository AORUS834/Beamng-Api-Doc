# Documentation for gui.lua

## texObj
Returns a table with the loaded texture information
@param path the path to a texture image
**Parameters:** path
**Examples:**
```lua
texObj("example.png")
```

## getFileName
**Parameters:** path, withoutExtension
**Examples:**
```lua
getFileName("example.png", "Example")
```

## getDefaultIconButtonSize
**Parameters:** None
**Examples:**
```lua
getDefaultIconButtonSize()
```

## setDefaultIconButtonSize
**Parameters:** size
**Examples:**
```lua
setDefaultIconButtonSize(32)
```

## createIconAtlas
Load and create the editor icon texture atlas. It also creates the editor.icons table with all the icons.
**Parameters:** None
**Examples:**
```lua
createIconAtlas()
```

## uiTextUnformattedRightAlign
**Parameters:** string_label, bool_sameLine, offset
**Examples:**
```lua

```

## uiTextColoredWithFont
**Parameters:** color, text, fontName
**Examples:**
```lua
uiTextColoredWithFont(imgui.ImVec4(1,1,1,1), "Example", nil)
```

## uiButtonRightAlign
**Parameters:** string_label, ImVec2_size, bool_sameLine, id, offset
**Examples:**
```lua
uiButtonRightAlign("Example", 32, nil, 1, nil)
```

## uiIconImage
Draw an icon image widget.
**Parameters:** icon, size, col, borderCol, label
**Examples:**
```lua
uiIconImage(nil, 32, nil, nil, "Example")
```

## uiHighlightedText
**Parameters:** text, highlightText, textColor
**Examples:**
```lua
uiHighlightedText("Example", "Example", imgui.ImVec4(1,1,1,1))
```

## uiIconImageButton
Draw an icon image button widget.
**Parameters:** icon, size, col, label, backgroundCol, id, textColor, textBG, onRelease, highlightText
**Examples:**
```lua
uiIconImageButton(nil, 32, nil, "Example", nil, 1, imgui.ImVec4(1,1,1,1), "Example", nil, "Example")
```

## uiHelpButton
**Parameters:** topicName, relativeUrl, size
**Examples:**
```lua
uiHelpButton(nil, nil, 32)
```

## showVizHelperWindow
Show the visibility helper tool window.
**Parameters:** None
**Examples:**
```lua
showVizHelperWindow()
```

## uiVertSeparator
**Parameters:** float_height, vec2_offset, width
**Examples:**
```lua
uiVertSeparator(nil, nil, 1)
```

## drawBrushSolidEdgeEllipse
**Parameters:** pos, fromPoint, toPoint, color
**Examples:**
```lua
drawBrushSolidEdgeEllipse(nil, nil, nil, imgui.ImVec4(1,1,1,1))
```

## drawBrushSolidEdgeBox
**Parameters:** fromPoint, toPoint, offset, color
**Examples:**
```lua
drawBrushSolidEdgeBox(nil, nil, nil, imgui.ImVec4(1,1,1,1))
```

## drawBrush
**Parameters:** brushType, pos, radius, numberOfSegments, color, terrainBlock, brushRatio, brushRotation, onlyTerrain
**Examples:**
```lua
drawBrush(nil, nil, nil, nil, imgui.ImVec4(1,1,1,1), nil, nil, nil, nil)
```

## windowResized
**Parameters:** size
**Examples:**
```lua
windowResized(32)
```

## checkWindowResize
Check if the main window got resized. It will call extensions hook onWindowResized with the new size as imgui ImVec2 as parameter.
**Parameters:** None
**Examples:**
```lua
checkWindowResize()
```

## isViewportHovered
Returns true if the 3D game viewport is hovered only.
**Parameters:** None
**Examples:**
```lua
isViewportHovered()
```

## isViewportFocused
**Parameters:** None
**Examples:**
```lua
isViewportFocused()
```

## presentGui
Used by editor, present the entire editor UI
**Parameters:** dtReal, dtSim, dtRaw
**Examples:**
```lua
presentGui(nil, nil, nil)
```

## screenToClient
**Parameters:** pt2i
**Examples:**
```lua
screenToClient(nil)
```

## uiDragFloat

Editing Wrappers

**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragFloat("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragFloat2
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragFloat2("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragFloat3
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragFloat3("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragFloat4
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragFloat4("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragFloatRange2
**Parameters:** label, v_current_min, v_current_max, v_speed, v_min, v_max, format, format_max, flags, editEnded
**Examples:**
```lua
uiDragFloatRange2("Example", nil, nil, nil, nil, nil, nil, nil, nil, nil)
```

## uiDragInt
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragInt("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragInt2
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragInt2("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragInt3
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragInt3("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragInt4
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragInt4("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiDragIntRange2
**Parameters:** label, v_current_min, v_current_max, v_speed, v_min, v_max, format, format_max, flags, editEnded
**Examples:**
```lua
uiDragIntRange2("Example", nil, nil, nil, nil, nil, nil, nil, nil, nil)
```

## uiDragScalar
**Parameters:** label, data_type, v, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragScalar("Example", nil, nil, nil, nil, nil, nil, nil, nil)
```

## uiDragScalarN
**Parameters:** label, data_type, v, components, v_speed, v_min, v_max, format, flags, editEnded
**Examples:**
```lua
uiDragScalarN("Example", nil, nil, nil, nil, nil, nil, nil, nil, nil)
```

## uiInputText
Widgets: Input with Keyboard
**Parameters:** label, buf, buf_size, flags, callback, user_data, editEnded
**Examples:**
```lua
uiInputText("Example", nil, 32, nil, nil, nil, nil)
```

## uiInputTextMultiline
**Parameters:** label, buf, buf_size, size, flags, callback, user_data, editEnded
**Examples:**
```lua
uiInputTextMultiline("Example", nil, 32, 32, nil, nil, nil, nil)
```

## uiInputTextMultilineReadOnly
**Parameters:** label, buf, size, flags, callback, user_data, editEnded
**Examples:**
```lua
uiInputTextMultilineReadOnly("Example", nil, 32, nil, nil, nil, nil)
```

## uiInputFloat
**Parameters:** label, v, step, step_fast, format, extra_flags, editEnded
**Examples:**
```lua
uiInputFloat("Example", nil, nil, nil, nil, nil, nil)
```

## uiInputFloat2
**Parameters:** label, v, format, extra_flags, editEnded
**Examples:**
```lua
uiInputFloat2("Example", nil, nil, nil, nil)
```

## uiInputFloat3
**Parameters:** label, v, format, extra_flags, editEnded
**Examples:**
```lua
uiInputFloat3("Example", nil, nil, nil, nil)
```

## uiInputFloat4
**Parameters:** label, v, format, extra_flags, editEnded
**Examples:**
```lua
uiInputFloat4("Example", nil, nil, nil, nil)
```

## uiInputInt
**Parameters:** label, v, step, step_fast, extra_flags, editEnded
**Examples:**
```lua
uiInputInt("Example", nil, nil, nil, nil, nil)
```

## uiInputInt2
**Parameters:** label, v, extra_flags, editEnded
**Examples:**
```lua
uiInputInt2("Example", nil, nil, nil)
```

## uiInputInt3
**Parameters:** label, v, extra_flags, editEnded
**Examples:**
```lua
uiInputInt3("Example", nil, nil, nil)
```

## uiInputInt4
**Parameters:** label, v, extra_flags, editEnded
**Examples:**
```lua
uiInputInt4("Example", nil, nil, nil)
```

## uiInputDouble
**Parameters:** label, v, step, step_fast, format, extra_flags, editEnded
**Examples:**
```lua
uiInputDouble("Example", nil, nil, nil, nil, nil, nil)
```

## uiInputScalar
**Parameters:** label, data_type, v, step, step_fast, format, extra_flags, editEnded
**Examples:**
```lua
uiInputScalar("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiInputScalarN
**Parameters:** label, data_type, v, components, step, step_fast, format, extra_flags, editEnded
**Examples:**
```lua
uiInputScalarN("Example", nil, nil, nil, nil, nil, nil, nil, nil)
```

## uiInputSearch
**Parameters:** label, text, width, extra_flags, editEnded
**Examples:**
```lua
uiInputSearch("Example", "Example", 1, nil, nil)
```

## uiInputSearchTextFilter
**Parameters:** label, txtfilter, width, extra_flags, editEnded
**Examples:**
```lua
uiInputSearchTextFilter("Example", nil, 1, nil, nil)
```

## uiInputFile
**Parameters:** label, buf, width, dir, extFilter, flags, editEnded
**Examples:**
```lua
uiInputFile("Example", nil, 1, nil, nil, nil, nil)
```

## uiSliderFloat
Widgets: Sliders
**Parameters:** label, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiSliderFloat("Example", nil, nil, nil, nil, nil, nil)
```

## uiSliderFloat2
**Parameters:** label, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiSliderFloat2("Example", nil, nil, nil, nil, nil, nil)
```

## uiSliderFloat3
**Parameters:** label, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiSliderFloat3("Example", nil, nil, nil, nil, nil, nil)
```

## uiSliderFloat4
**Parameters:** label, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiSliderFloat4("Example", nil, nil, nil, nil, nil, nil)
```

## uiSliderAngle
**Parameters:** label, v_rad, v_degrees_min, v_degrees_max, editEnded
**Examples:**
```lua
uiSliderAngle("Example", nil, nil, nil, nil)
```

## uiSliderInt
**Parameters:** label, v, v_min, v_max, format, editEnded
**Examples:**
```lua
uiSliderInt("Example", nil, nil, nil, nil, nil)
```

## uiSliderInt2
**Parameters:** label, v, v_min, v_max, format, editEnded
**Examples:**
```lua
uiSliderInt2("Example", nil, nil, nil, nil, nil)
```

## uiSliderInt3
**Parameters:** label, v, v_min, v_max, format, editEnded
**Examples:**
```lua
uiSliderInt3("Example", nil, nil, nil, nil, nil)
```

## uiSliderInt4
**Parameters:** label, v, v_min, v_max, format, editEnded
**Examples:**
```lua
uiSliderInt4("Example", nil, nil, nil, nil, nil)
```

## uiSliderScalar
**Parameters:** label, data_type, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiSliderScalar("Example", nil, nil, nil, nil, nil, nil, nil)
```

## uiSliderScalarN
**Parameters:** label, data_type, v, components, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiSliderScalarN("Example", nil, nil, nil, nil, nil, nil, nil, nil)
```

## uiVSliderFloat
**Parameters:** label, size, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiVSliderFloat("Example", 32, nil, nil, nil, nil, nil, nil)
```

## uiVSliderInt
**Parameters:** label, size, v, v_min, v_max, format, editEnded
**Examples:**
```lua
uiVSliderInt("Example", 32, nil, nil, nil, nil, nil)
```

## uiVSliderScalar
**Parameters:** label, size, data_type, v, v_min, v_max, format, power, editEnded
**Examples:**
```lua
uiVSliderScalar("Example", 32, nil, nil, nil, nil, nil, nil, nil)
```

## uiColorEdit3
Widgets: Color Editor/Picker
**Parameters:** label, col, flags, editEnded
**Examples:**
```lua
uiColorEdit3("Example", nil, nil, nil)
```

## uiColorEdit4
**Parameters:** label, col, flags, editEnded
**Examples:**
```lua
uiColorEdit4("Example", nil, nil, nil)
```

## uiColorEdit8
**Parameters:** label, col, flags, editEnded
**Examples:**
```lua
uiColorEdit8("Example", nil, nil, nil)
```

## uiColorPicker3
**Parameters:** label, col, flags, editEnded
**Examples:**
```lua
uiColorPicker3("Example", nil, nil, nil)
```

## uiColorPicker4
**Parameters:** label, col, flags, ref_col, editEnded
**Examples:**
```lua
uiColorPicker4("Example", nil, nil, nil, nil)
```

## uiColorButton
**Parameters:** desc_id, col, flags, size, editEnded
**Examples:**
```lua
uiColorButton(1, nil, nil, 32, nil)
```

## uiPlotLines1
**Parameters:** string_label, float_values, int_values_count, int_values_offset, string_overlay_text, float_scale_min, float_scale_max, ImVec2_graph_size, int_stride, auto_resize
**Examples:**
```lua
uiPlotLines1("Example", nil, nil, nil, "Example", nil, nil, 32, 1, 32)
```

## IsItemDoubleClicked
**Parameters:** int_mouse_button
**Examples:**
```lua
IsItemDoubleClicked(nil)
```

## IsItemClicked
**Parameters:** int_mouse_button
**Examples:**
```lua
IsItemClicked(nil)
```

## getFontList
Returns a table with all the fonts imgui has available
**Parameters:** None
**Examples:**
```lua
getFontList()
```

## registerWindow
Register a given window name, usually must be called in onEditorInitialized() of the editor extension.
For more usage of the window api, @see [Tutorial - Step #2, Writing base code](../../../../tutorials/world_editor/create_editor_tool/_index.md).
@param windowName the name of the window to register
@param defaultSize the default first time size of the window, as imgui ImVec2
@param defaultPos the default first time size of the window, as imgui ImVec2
@param defaultVisibleBoolean if this is not nil, it will be the default first time open state of the window
@param modal if the window is a modal window
@param centered if the window is centered by default
**Parameters:** windowName, defaultSize, defaultPos, defaultVisibleBoolean, modal, centered, groupName
**Examples:**
```lua
registerWindow(nil, 32, nil, nil, nil, nil, nil)
```

## isWindowRegistered
**Parameters:** windowName
**Examples:**
```lua
isWindowRegistered(nil)
```

## registerModalWindow
Register a given modal window name, usually must be called in onEditorInitialized() of the editor extension.
For more usage of the window api, @see [Tutorial - Step #2, Writing base code](../../../../tutorials/world_editor/create_editor_tool/_index.md).
@param windowName the name of the window to register
@param defaultSize the default first time size of the window, as imgui ImVec2
@param defaultPos the default first time size of the window, as imgui ImVec2
@param defaultVisibleBoolean if this is not nil, it will be the default first time open state of the window
@param centered if the window is centered by default
**Parameters:** windowName, defaultSize, defaultPos, centered
**Examples:**
```lua
registerModalWindow(nil, 32, nil, nil)
```

## checkAndTriggerWindowHooks
**Parameters:** wndName, wnd
**Examples:**
```lua
checkAndTriggerWindowHooks(nil, nil)
```

## unregisterWindow
Unregister a given window name. For example when a tool window was closed, you dont want it in the saved state of the editor anymore.
Call this function right after the imgui.Begin call, if the editor.isWindowVisible(yourWindowName) is false.
If you just want to hide the window, the call editor.hideWindow(yourWindowName) only.
For more usage of the window api, see [Tutorial - Step #2, Writing base code](../../../../tutorials/world_editor/create_editor_tool/_index.md).
@param windowName the name of the window to unregister
**Parameters:** windowName
**Examples:**
```lua
unregisterWindow(nil)
```

## isWindowVisible
**Parameters:** windowName
**Examples:**
```lua
isWindowVisible(nil)
```

## getWindowVisibleBoolPtr
Return the boolean pointer of imgui which stores the visibility of the window, used in imgui.Begin call.
@param windowName the name of the window
**Parameters:** windowName
**Examples:**
```lua
getWindowVisibleBoolPtr(nil)
```

## hideWindow
Hide the named window, sets the visible boolean to false.
@param windowName the name of the window
**Parameters:** windowName
**Examples:**
```lua
hideWindow(nil)
```

## hideAllWindows
Hide all registered windows
**Parameters:** None
**Examples:**
```lua
hideAllWindows()
```

## showWindow
Show the named window, sets the visible boolean to false.
@param windowName the name of the window
**Parameters:** windowName, show
**Examples:**
```lua
showWindow(nil, nil)
```

## setWindowVisibility
**Parameters:** windowName, visible
**Examples:**
```lua
setWindowVisibility(nil, nil)
```

## setWindowGroupVisibility
**Parameters:** groupName, visible
**Examples:**
```lua
setWindowGroupVisibility(nil, nil)
```

## setupWindow
Setup the window's default size and position. Must be called before imgui.Begin.
@param windowName the name of the window
**Parameters:** windowName
**Examples:**
```lua
setupWindow(nil)
```

## checkWindowFocus
**Parameters:** windowName
**Examples:**
```lua
checkWindowFocus(nil)
```

## beginWindow
**Parameters:** windowName, title, flags, noClose
**Examples:**
```lua
beginWindow(nil, nil, nil, nil)
```

## beginModalWindow
**Parameters:** windowName, title, flags, noClose
**Examples:**
```lua
beginModalWindow(nil, nil, nil, nil)
```

## endWindow
**Parameters:** None
**Examples:**
```lua
endWindow()
```

## endModalWindow
**Parameters:** None
**Examples:**
```lua
endModalWindow()
```

## openModalWindow
**Parameters:** windowName
**Examples:**
```lua
openModalWindow(nil)
```

## closeModalWindow
**Parameters:** windowName
**Examples:**
```lua
closeModalWindow(nil)
```

## saveWindowsState
**Parameters:** customFilename
**Examples:**
```lua
saveWindowsState("example.png")
```

## loadWindowsState
**Parameters:** customFilename, toolName
**Examples:**
```lua
loadWindowsState("example.png", nil)
```

## callShowWindowHookForVisibleWindows
**Parameters:** None
**Examples:**
```lua
callShowWindowHookForVisibleWindows()
```

## defocusFocusedWindow
**Parameters:** None
**Examples:**
```lua
defocusFocusedWindow()
```

## setWindowGroup
**Parameters:** windowName, groupName
**Examples:**
```lua
setWindowGroup(nil, nil)
```

## openModalDialog
**Parameters:** title, windowSize, uiFunction
**Examples:**
```lua
openModalDialog(nil, 32, nil)
```

## closeModalDialog
**Parameters:** None
**Examples:**
```lua
closeModalDialog()
```

## modalDialogWindowUi
called by the editor, internal
**Parameters:** None
**Examples:**
```lua
modalDialogWindowUi()
```

## addWindowsStateApi
**Parameters:** None
**Examples:**
```lua
addWindowsStateApi()
```

## addGuiCoreApi
**Parameters:** None
**Examples:**
```lua
addGuiCoreApi()
```

## addUndoReadyWidgetsApi
**Parameters:** None
**Examples:**
```lua
addUndoReadyWidgetsApi()
```

## uiInputFloatEx_componentInput
**Parameters:** v, v_index, widgetId, step_buttons, step, step_fast, format, intermediate, editEnded, componentWidth
**Examples:**
```lua
uiInputFloatEx_componentInput(nil, nil, 1, nil, nil, nil, nil, nil, nil, 1)
```

## uiInputFloatEx
**Parameters:** label, v, step, step_fast, format, flags, editEnded
**Examples:**
```lua
uiInputFloatEx("Example", nil, nil, nil, nil, nil, nil)
```

## uiInputFloat2Ex
**Parameters:** label, v, step, step_fast, format, flags, editEnded
**Examples:**
```lua
uiInputFloat2Ex("Example", nil, nil, nil, nil, nil, nil)
```

## uiInputFloat3Ex
**Parameters:** label, v, step, step_fast, format, flags, editEnded
**Examples:**
```lua
uiInputFloat3Ex("Example", nil, nil, nil, nil, nil, nil)
```

## uiInputFloat4Ex
**Parameters:** label, v, step, step_fast, format, flags, editEnded
**Examples:**
```lua
uiInputFloat4Ex("Example", nil, nil, nil, nil, nil, nil)
```

## addExWidgetsApi
**Parameters:** None
**Examples:**
```lua
addExWidgetsApi()
```

## addOtherWidgetsApi
**Parameters:** None
**Examples:**
```lua
addOtherWidgetsApi()
```

## getTempBool_BoolBool
in: bool, out: bool pointer
in: nil, out: bool
**Parameters:** value
**Examples:**
```lua
getTempBool_BoolBool(nil)
```

## getTempBool_StringString
in string; out bool pointer
in nil; out string
**Parameters:** value
**Examples:**
```lua
getTempBool_StringString(nil)
```

## getTempInt_NumberNumber
in: number, out: int pointer
in: nil, out: number
**Parameters:** value
**Examples:**
```lua
getTempInt_NumberNumber(nil)
```

## getTempInt_StringString
in string; out int pointer
in nil; out number
**Parameters:** value
**Examples:**
```lua
getTempInt_StringString(nil)
```

## getTempIntArray2_StringString
in string; out int pointer/array
in nil; out string
**Parameters:** value
**Examples:**
```lua
getTempIntArray2_StringString(nil)
```

## getTempFloat_NumberNumber
in: number, out: float pointer
in: nil, out: number
**Parameters:** value
**Examples:**
```lua
getTempFloat_NumberNumber(nil)
```

## getTempFloat_StringString
in string; out float pointer
in nil; out number
**Parameters:** value
**Examples:**
```lua
getTempFloat_StringString(nil)
```

## getTempFloatArray2_StringString
in string; out float pointer/array
in nil; out string
**Parameters:** value
**Examples:**
```lua
getTempFloatArray2_StringString(nil)
```

## getTempFloatArray2_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value
**Examples:**
```lua
getTempFloatArray2_TableTable(nil)
```

## getTempFloatArray3_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value
**Examples:**
```lua
getTempFloatArray3_TableTable(nil)
```

## getTempFloatArray3_Vec3Vec3
**Parameters:** value
**Examples:**
```lua
getTempFloatArray3_Vec3Vec3(nil)
```

## getTempFloatArray4_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value
**Examples:**
```lua
getTempFloatArray4_TableTable(nil)
```

## getTempFloatArray4_StringString
in string; out float pointer/array
in nil; out string
**Parameters:** value
**Examples:**
```lua
getTempFloatArray4_StringString(nil)
```

## getTempImVec4_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value
**Examples:**
```lua
getTempImVec4_TableTable(nil)
```

## getTempCharPtr
in string; out char pointer
in nil; out string
**Parameters:** value
**Examples:**
```lua
getTempCharPtr(nil)
```

## getTempTextureObj
in: string/path, out: texture object
in: nil, out: texture object
**Parameters:** value
**Examples:**
```lua
getTempTextureObj(nil)
```

## getTempImVec4_TableImVec4
in table; out float ImVec4
in nil; out ImVec4
**Parameters:** value
**Examples:**
```lua
getTempImVec4_TableImVec4(nil)
```

## addCTypeHelperApi
**Parameters:** None
**Examples:**
```lua
addCTypeHelperApi()
```

## setKeyModifier
**Parameters:** mod, pressed
**Examples:**
```lua
setKeyModifier(nil, nil)
```

## uiRenderAlternateRows
Render alternate-color rows current window/child
Based on approach in https://github.com/ocornut/imgui/issues/2668
IMPORTANT: Requires to be surrounded by Begin/BeginChild, End/EndChild
**Parameters:** lineHeight, mOddColor, mEvenColor
**Examples:**
```lua
uiRenderAlternateRows(nil, imgui.ImVec4(1,1,1,1), imgui.ImVec4(1,1,1,1))
```

## testOddImColor
**Parameters:** None
**Examples:**
```lua
testOddImColor()
```

## testOddImVec4
**Parameters:** None
**Examples:**
```lua
testOddImVec4()
```

## testEvenImColor
**Parameters:** None
**Examples:**
```lua
testEvenImColor()
```

## testEvenImVec4
**Parameters:** None
**Examples:**
```lua
testEvenImVec4()
```

## initialize
**Parameters:** editorInstance
**Examples:**
```lua
initialize(nil)
```

