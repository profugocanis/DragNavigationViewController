### DragNavigationViewController

`DragNavigationViewController.swift` is a custom UIViewController container that enables a drag-to-dismiss interaction across the entire screen. Unlike traditional navigation controllers that limit gesture handling to specific areas, `DragNavigationViewController.swift` allows users to swipe or drag anywhere on the screen to dismiss the view controller. This provides a more fluid and intuitive way for users to exit the current view, enhancing the overall interaction experience.

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
