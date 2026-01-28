# Documentation for gui.lua

## texObj
Returns a table with the loaded texture information
@param path the path to a texture image
**Parameters:** path

## getFileName
**Parameters:** path, withoutExtension

## getDefaultIconButtonSize
**Parameters:** None

## setDefaultIconButtonSize
**Parameters:** size

## createIconAtlas
Load and create the editor icon texture atlas. It also creates the editor.icons table with all the icons.
**Parameters:** None

## uiTextUnformattedRightAlign
**Parameters:** string_label, bool_sameLine, offset

## uiTextColoredWithFont
**Parameters:** color, text, fontName

## uiButtonRightAlign
**Parameters:** string_label, ImVec2_size, bool_sameLine, id, offset

## uiIconImage
Draw an icon image widget.
**Parameters:** icon, size, col, borderCol, label

## uiHighlightedText
**Parameters:** text, highlightText, textColor

## uiIconImageButton
Draw an icon image button widget.
**Parameters:** icon, size, col, label, backgroundCol, id, textColor, textBG, onRelease, highlightText

## uiHelpButton
**Parameters:** topicName, relativeUrl, size

## showVizHelperWindow
Show the visibility helper tool window.
**Parameters:** None

## uiVertSeparator
**Parameters:** float_height, vec2_offset, width

## drawBrushSolidEdgeEllipse
**Parameters:** pos, fromPoint, toPoint, color

## drawBrushSolidEdgeBox
**Parameters:** fromPoint, toPoint, offset, color

## drawBrush
**Parameters:** brushType, pos, radius, numberOfSegments, color, terrainBlock, brushRatio, brushRotation, onlyTerrain

## windowResized
**Parameters:** size

## checkWindowResize
Check if the main window got resized. It will call extensions hook onWindowResized with the new size as imgui ImVec2 as parameter.
**Parameters:** None

## isViewportHovered
Returns true if the 3D game viewport is hovered only.
**Parameters:** None

## isViewportFocused
**Parameters:** None

## presentGui
Used by editor, present the entire editor UI
**Parameters:** dtReal, dtSim, dtRaw

## screenToClient
**Parameters:** pt2i

## uiDragFloat

Editing Wrappers

**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragFloat2
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragFloat3
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragFloat4
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragFloatRange2
**Parameters:** label, v_current_min, v_current_max, v_speed, v_min, v_max, format, format_max, flags, editEnded

## uiDragInt
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragInt2
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragInt3
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragInt4
**Parameters:** label, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragIntRange2
**Parameters:** label, v_current_min, v_current_max, v_speed, v_min, v_max, format, format_max, flags, editEnded

## uiDragScalar
**Parameters:** label, data_type, v, v_speed, v_min, v_max, format, flags, editEnded

## uiDragScalarN
**Parameters:** label, data_type, v, components, v_speed, v_min, v_max, format, flags, editEnded

## uiInputText
Widgets: Input with Keyboard
**Parameters:** label, buf, buf_size, flags, callback, user_data, editEnded

## uiInputTextMultiline
**Parameters:** label, buf, buf_size, size, flags, callback, user_data, editEnded

## uiInputTextMultilineReadOnly
**Parameters:** label, buf, size, flags, callback, user_data, editEnded

## uiInputFloat
**Parameters:** label, v, step, step_fast, format, extra_flags, editEnded

## uiInputFloat2
**Parameters:** label, v, format, extra_flags, editEnded

## uiInputFloat3
**Parameters:** label, v, format, extra_flags, editEnded

## uiInputFloat4
**Parameters:** label, v, format, extra_flags, editEnded

## uiInputInt
**Parameters:** label, v, step, step_fast, extra_flags, editEnded

## uiInputInt2
**Parameters:** label, v, extra_flags, editEnded

## uiInputInt3
**Parameters:** label, v, extra_flags, editEnded

## uiInputInt4
**Parameters:** label, v, extra_flags, editEnded

## uiInputDouble
**Parameters:** label, v, step, step_fast, format, extra_flags, editEnded

## uiInputScalar
**Parameters:** label, data_type, v, step, step_fast, format, extra_flags, editEnded

## uiInputScalarN
**Parameters:** label, data_type, v, components, step, step_fast, format, extra_flags, editEnded

## uiInputSearch
**Parameters:** label, text, width, extra_flags, editEnded

## uiInputSearchTextFilter
**Parameters:** label, txtfilter, width, extra_flags, editEnded

## uiInputFile
**Parameters:** label, buf, width, dir, extFilter, flags, editEnded

## uiSliderFloat
Widgets: Sliders
**Parameters:** label, v, v_min, v_max, format, power, editEnded

## uiSliderFloat2
**Parameters:** label, v, v_min, v_max, format, power, editEnded

## uiSliderFloat3
**Parameters:** label, v, v_min, v_max, format, power, editEnded

## uiSliderFloat4
**Parameters:** label, v, v_min, v_max, format, power, editEnded

## uiSliderAngle
**Parameters:** label, v_rad, v_degrees_min, v_degrees_max, editEnded

## uiSliderInt
**Parameters:** label, v, v_min, v_max, format, editEnded

## uiSliderInt2
**Parameters:** label, v, v_min, v_max, format, editEnded

## uiSliderInt3
**Parameters:** label, v, v_min, v_max, format, editEnded

## uiSliderInt4
**Parameters:** label, v, v_min, v_max, format, editEnded

## uiSliderScalar
**Parameters:** label, data_type, v, v_min, v_max, format, power, editEnded

## uiSliderScalarN
**Parameters:** label, data_type, v, components, v_min, v_max, format, power, editEnded

## uiVSliderFloat
**Parameters:** label, size, v, v_min, v_max, format, power, editEnded

## uiVSliderInt
**Parameters:** label, size, v, v_min, v_max, format, editEnded

## uiVSliderScalar
**Parameters:** label, size, data_type, v, v_min, v_max, format, power, editEnded

## uiColorEdit3
Widgets: Color Editor/Picker
**Parameters:** label, col, flags, editEnded

## uiColorEdit4
**Parameters:** label, col, flags, editEnded

## uiColorEdit8
**Parameters:** label, col, flags, editEnded

## uiColorPicker3
**Parameters:** label, col, flags, editEnded

## uiColorPicker4
**Parameters:** label, col, flags, ref_col, editEnded

## uiColorButton
**Parameters:** desc_id, col, flags, size, editEnded

## uiPlotLines1
**Parameters:** string_label, float_values, int_values_count, int_values_offset, string_overlay_text, float_scale_min, float_scale_max, ImVec2_graph_size, int_stride, auto_resize

## IsItemDoubleClicked
**Parameters:** int_mouse_button

## IsItemClicked
**Parameters:** int_mouse_button

## getFontList
Returns a table with all the fonts imgui has available
**Parameters:** None

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

## isWindowRegistered
**Parameters:** windowName

## registerModalWindow
Register a given modal window name, usually must be called in onEditorInitialized() of the editor extension.
For more usage of the window api, @see [Tutorial - Step #2, Writing base code](../../../../tutorials/world_editor/create_editor_tool/_index.md).
@param windowName the name of the window to register
@param defaultSize the default first time size of the window, as imgui ImVec2
@param defaultPos the default first time size of the window, as imgui ImVec2
@param defaultVisibleBoolean if this is not nil, it will be the default first time open state of the window
@param centered if the window is centered by default
**Parameters:** windowName, defaultSize, defaultPos, centered

## checkAndTriggerWindowHooks
**Parameters:** wndName, wnd

## unregisterWindow
Unregister a given window name. For example when a tool window was closed, you dont want it in the saved state of the editor anymore.
Call this function right after the imgui.Begin call, if the editor.isWindowVisible(yourWindowName) is false.
If you just want to hide the window, the call editor.hideWindow(yourWindowName) only.
For more usage of the window api, see [Tutorial - Step #2, Writing base code](../../../../tutorials/world_editor/create_editor_tool/_index.md).
@param windowName the name of the window to unregister
**Parameters:** windowName

## isWindowVisible
**Parameters:** windowName

## getWindowVisibleBoolPtr
Return the boolean pointer of imgui which stores the visibility of the window, used in imgui.Begin call.
@param windowName the name of the window
**Parameters:** windowName

## hideWindow
Hide the named window, sets the visible boolean to false.
@param windowName the name of the window
**Parameters:** windowName

## hideAllWindows
Hide all registered windows
**Parameters:** None

## showWindow
Show the named window, sets the visible boolean to false.
@param windowName the name of the window
**Parameters:** windowName, show

## setWindowVisibility
**Parameters:** windowName, visible

## setWindowGroupVisibility
**Parameters:** groupName, visible

## setupWindow
Setup the window's default size and position. Must be called before imgui.Begin.
@param windowName the name of the window
**Parameters:** windowName

## checkWindowFocus
**Parameters:** windowName

## beginWindow
**Parameters:** windowName, title, flags, noClose

## beginModalWindow
**Parameters:** windowName, title, flags, noClose

## endWindow
**Parameters:** None

## endModalWindow
**Parameters:** None

## openModalWindow
**Parameters:** windowName

## closeModalWindow
**Parameters:** windowName

## saveWindowsState
**Parameters:** customFilename

## loadWindowsState
**Parameters:** customFilename, toolName

## callShowWindowHookForVisibleWindows
**Parameters:** None

## defocusFocusedWindow
**Parameters:** None

## setWindowGroup
**Parameters:** windowName, groupName

## openModalDialog
**Parameters:** title, windowSize, uiFunction

## closeModalDialog
**Parameters:** None

## modalDialogWindowUi
called by the editor, internal
**Parameters:** None

## addWindowsStateApi
**Parameters:** None

## addGuiCoreApi
**Parameters:** None

## addUndoReadyWidgetsApi
**Parameters:** None

## uiInputFloatEx_componentInput
**Parameters:** v, v_index, widgetId, step_buttons, step, step_fast, format, intermediate, editEnded, componentWidth

## uiInputFloatEx
**Parameters:** label, v, step, step_fast, format, flags, editEnded

## uiInputFloat2Ex
**Parameters:** label, v, step, step_fast, format, flags, editEnded

## uiInputFloat3Ex
**Parameters:** label, v, step, step_fast, format, flags, editEnded

## uiInputFloat4Ex
**Parameters:** label, v, step, step_fast, format, flags, editEnded

## addExWidgetsApi
**Parameters:** None

## addOtherWidgetsApi
**Parameters:** None

## getTempBool_BoolBool
in: bool, out: bool pointer
in: nil, out: bool
**Parameters:** value

## getTempBool_StringString
in string; out bool pointer
in nil; out string
**Parameters:** value

## getTempInt_NumberNumber
in: number, out: int pointer
in: nil, out: number
**Parameters:** value

## getTempInt_StringString
in string; out int pointer
in nil; out number
**Parameters:** value

## getTempIntArray2_StringString
in string; out int pointer/array
in nil; out string
**Parameters:** value

## getTempFloat_NumberNumber
in: number, out: float pointer
in: nil, out: number
**Parameters:** value

## getTempFloat_StringString
in string; out float pointer
in nil; out number
**Parameters:** value

## getTempFloatArray2_StringString
in string; out float pointer/array
in nil; out string
**Parameters:** value

## getTempFloatArray2_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value

## getTempFloatArray3_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value

## getTempFloatArray3_Vec3Vec3
**Parameters:** value

## getTempFloatArray4_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value

## getTempFloatArray4_StringString
in string; out float pointer/array
in nil; out string
**Parameters:** value

## getTempImVec4_TableTable
in table; out float pointer/array
in nil; out table
**Parameters:** value

## getTempCharPtr
in string; out char pointer
in nil; out string
**Parameters:** value

## getTempTextureObj
in: string/path, out: texture object
in: nil, out: texture object
**Parameters:** value

## getTempImVec4_TableImVec4
in table; out float ImVec4
in nil; out ImVec4
**Parameters:** value

## addCTypeHelperApi
**Parameters:** None

## setKeyModifier
**Parameters:** mod, pressed

## uiRenderAlternateRows
Render alternate-color rows current window/child
Based on approach in https://github.com/ocornut/imgui/issues/2668
IMPORTANT: Requires to be surrounded by Begin/BeginChild, End/EndChild
**Parameters:** lineHeight, mOddColor, mEvenColor

## testOddImColor
**Parameters:** None

## testOddImVec4
**Parameters:** None

## testEvenImColor
**Parameters:** None

## testEvenImVec4
**Parameters:** None

## initialize
**Parameters:** editorInstance

