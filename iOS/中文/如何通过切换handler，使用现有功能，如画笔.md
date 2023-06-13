### 如何通过切换handler，使用现有功能，如画笔

```objc
id<IToolHandler> toolHandler = [self.extensionsMgr getToolHandlerByName:Tool_Link];
self.extensionsMgr.currentToolHandler = toolHandler;
```
`ToolHandlerName`可参考`<uiextensionsDynamic/FSUtilities.h>`
![截图1](/iOS/ScreenCapture/20230613174112.jpg)


### 如何切换状态，启用现有功能，如搜索功能

```objc
[self.extensionsMgr changeState:FSUIManagerStateSearch];
```
`state`可参考`<uiextensionsDynamic/FSUtilities.h>`
![截图1](/iOS/ScreenCapture/20230613174427.jpg)