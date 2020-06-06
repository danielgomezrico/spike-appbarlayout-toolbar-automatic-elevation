# MaterialComponents, CoordinatorLayout, AppBarLayout, Toolbar and automatic elevation Spike

Here's an example of how to use themes to get automatic `Toolbar` elevation without extra code or custom listeners.

Use [AppBarLayout](https://developer.android.com/reference/com/google/android/material/appbar/AppBarLayout)
from [MaterialComponents](https://github.com/material-components/material-components-android) for it.

# How to

1. Your app style should use a `MaterialCompoment` style, like [src/main/res/values/styles.xml](src/main/res/values/styles.xml).
2. Setup you AppBarLayout:
   * Use any MaterialCompoments style for this component like: `Widget.MaterialComponents.AppBarLayout.Surface`.
   * Set `app:liftOnScroll="true"` to enable the automatic elevation based on scroll.

3. Setup your scrolling view:
   * Set `app:layout_behavior="@string/appbar_scrolling_view_behavior`.

And that's all :)

# Results

![](example.gif)
