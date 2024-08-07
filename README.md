### DragNavigationViewController

#### Use
- Add [SwiftUIIntrospect](https://github.com/siteline/swiftui-introspect) to Your Project;
- Add `DragNavigationViewController.swift` to Your Project;
- Subclass UINavigationController:

```Swift
class CustomNavigationController: DragNavigationViewController {
   ...
}
```

#### Use with SwiftUI.TabView
```Swift
TabView(selection: $selectedIndex) {
   ...
}
.setupWithNavigationGesture(position: selectedIndex)
```

#### Disable gesture
```Swift
dragNavigationViewController.isEnabledPopGestureRecognizer = false
```

#### Set StatusBarStyle
```Swift
dragNavigationViewController.setStatusBarStyle(.lightContent)
```
