### DragNavigationViewController

#### Use
- Add [SwiftUIIntrospect](https://github.com/siteline/swiftui-introspect) to Your Project;
- Add `DragNavigationViewController.swift` to Your Project;
- Subclass UINavigationController:

```Swift
import UIKit

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
