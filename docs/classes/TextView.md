**super**: **[UITextView](UITextView.md)** (on iOS)

The TextView class implements the behavior for a scrollable, multiline text region. The class supports the display of text using custom style information and also supports text editing. You typically use a text view to display multiple lines of text, such as when displaying the body of a large text document.

### Events

* **Load**()
This event is called when the object becames available in the current runtime system.

* **DidBeginEditing**()
Use this event to be notified when editing began in the specified text field.

* **DidEndEditing**()
Use this event to be notified when editing stopped for the specified text field.

* **Changed**()
Use this event to be notified when text changed in the specified text field.

* **DidChangeSelection**()
Use this event to be notified when text selection changed in the specified text field.

* **DidScroll**()
This event is called when the user scrolls the content view.

* **DidEndDragging**(**decelerate**: **[Bool](../gravity/types.md)**)
This event is called when dragging ended in the scroll view. The scroll view sends this event when the user’s finger touches up after dragging content. The decelerating property of the scroll view controls deceleration. The decelerate value is true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is NO, scrolling stops immediately upon touch-up.

* **DidEndDecelerating**()
This event is called when the scroll view ends decelerating the scrolling movement.

* **Unload**()
This event is called when the object has been removed from the current runtime system (but not yet deallocated).



### Properties

* **var** **text**: **[String](../gravity/types.md)**
The text displayed by the text view.

* **var** **rawText**: **[String](../gravity/types.md)**
The raw text currently set in the text view. \(read-only\)

* **var** **textColor**: **[Color](Color.md)**
The color of the text.

* **var** **textType**: **TextType**
A value that specifies how text must be interpreted and rendered.

* **var** **font**: **[Font](Font.md)**
The font of the text.

* **var** **textAlignment**: **TextAlignment**
The technique to use for aligning the text.

* **var** **selectedRange**: **[Range](../gravity/types.md)**
The current selection range of the receiver.

* **var** **editable**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether the receiver is editable.

* **var** **dataDetectorTypes**: **DataDetectorTypes**
The types of data converted to tappable URLs in the text view.

* **var** **clearsOnInsertion**: **[Bool](../gravity/types.md)**
A Boolean value indicating whether inserting text replaces the previous contents.

* **var** **inputView**: **[UIView](UIView.md)**
The custom input view to display when the text view becomes the first responder.

* **var** **inputAccessoryView**: **[UIView](UIView.md)**
The custom accessory view to display when the text view becomes the first responder.



### Methods

* **func** **hasText**(): <strong>[Bool](../gravity/types.md)</strong> 
Returns a Boolean value indicating whether the text view currently contains any text.

* **func** **appendText**(**text**: **[String](../gravity/types.md)**)
Appends a given string to the receiver.

* **func** **scrollRangeToVisible**(**range**: **[Range](../gravity/types.md)**)
Scrolls the receiver until the text in the specified range is visible.

* **func** **animate**(**duration**: **[Float](../gravity/types.md)**, **delay**: **[Float](../gravity/types.md)**, **options**: **<a href="#_enum_AnimationOption">AnimationOption</a>**, **closure**: **[Closure](../gravity/closure.md)**, **completion**: **[Closure](../gravity/closure.md)**)
Animate changes to one or more views using the specified duration, delay, options and completion handler.

* **func** **setFocus**()
Force focus to be set to the selected control. For TextField and TextView that means force Keyboard to appear.

* **func** **clearFocus**()
Clear focus from selected control





### Enumeration

#### TextType
 * .HTML
 * .Markdown
 * .Text

#### TextAlignment
 * .Center
 * .Justified
 * .Left
 * .Natural
 * .Right

#### DataDetectorTypes
 * .Address
 * .All
 * .CalendarEvent
 * .Link
 * .None
 * .PhoneNumber

#### AnimationOption
 * .AllowAnimatedContent
 * .AllowUserInteraction
 * .Autoreverse
 * .BeginFromCurrentState
 * .CurveEaseIn
 * .CurveEaseInOut
 * .CurveEaseOut
 * .CurveLinear
 * .LayoutSubviews
 * .OverrideInheritedCurve
 * .OverrideInheritedDuration
 * .OverrideInheritedOptions
 * .Repeat
 * .ShowHideTransitionViews
 * .TransitionCrossDissolve
 * .TransitionCurlDown
 * .TransitionCurlUp
 * .TransitionFlipFromBottom
 * .TransitionFlipFromLeft
 * .TransitionFlipFromRight
 * .TransitionFlipFromTop
 * .TransitionNone



