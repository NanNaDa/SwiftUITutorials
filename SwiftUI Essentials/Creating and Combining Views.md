# Creating and Combining Views
  This tutorial guides you through building _Landmarks_ -- an iOS app for discovering and sharing the places you love. You'll start by building the view that shows a landmark's details.

  To lay out the views, Landmarks uses stacks to combine and layer the image and text view components. To add a map to the view, you'll include a standard MapKit component. As you refine the view's design, Xcode provides real-time feedback so you can see how those changes translate into code.

  Download the project files to begin building this project, and follow the steps below.

## section 1
**Create a New Project and Explore the Canvas**

  Create a new Xcode project that uses SwiftUI. Explore the canvas, previews, and the SwiftUI template code.

  To preview and interact with views from the canvas in Xcode, ensure your Mac is running macOS Catalina 10.15.


### Step 1
  Open Xcode and either click **Create a new Xcode project** in Xcode's startup window, or choose **File > New > Project.**

### Step 2
  In the template selector, select **iOS** as the platform, select the **Single View App** template, and then click **Next.**

### Step 3
  Enter "Landmarks" as the Product Name, select **SwiftUI**for the user interface, and click **Next**. Choose a location to save the landmarks project on your Mac.

### Step 4
  In the Project navigator, select ContentView.swift.

  By default, SwiftUI view files declare two structures. The first structure conforms to the View protocol and describes the view's content and layout. The second structure declares a preview for that view.

### Step 5
  In the canvas, click **Resume** to display the preview.

  **Tip**
  If the canvas isn't visible, select **Editor > Editor and Canvas** to show it.

### Step 6
  Inside the body property, change "Hello world" to a greeting for yourself.
  
  As you change the code in a view's body property, the preview  updates to reflect your changes.


## Section 2
**Customize the Text View**

  You can customize a view's display by changing your code, or by using the inspector to discover what's available and to help you write code.
  
  As you build the Landmarks app, you can use any combination of editors: the source editor, the canvas, or the inspectors. Your code stays updated, regardless of which tool you use.
  
  Next, you'll customize the text view using the inspector.
  
### Step 1
  In the preview, Command-click the greeting to bring up the structured editing popover, and choose **Inspect**.
  
  The popover shows different attributes that you can customize, depending on the type of view you inspect.
  
### Step 2
  Use the inspector to change the text to "Turtle Rock", the name of the first landmark you'll show in your app.
  
### Step 3
  Change the Font modifier to **Title**.
  
  This applies the system font to the text so that it responds correctly to the user's preferred font sizes and settings.
  
  To customize a SwiftUI view, you call methods called _modifiers_. Modifiers wrap a view to change its display or other properties. Each modifier returns a new view, so it's common to chain multiple modifiers, stacked vertically.
  
### Step 4
  Edit the code by hand to add the foregroundColor(.green) modifier; this changes the text's color to green.
  
  Your code is always the source of truth for the view. When you use the inspector to change or remove a modifier, Xcode updates your code immediately to match.
  
### Step 5
  This time, open the inspector by Command-clicking on the Text declaration in the code eidtor, and then choose **Inspect** from the popover. Click the **Color** pop-up menu and choose **Inherited** to change the text color to black again.
  
### Step 6
  Notice that Xcode updates your code automatically to reflect the change, removing the foregroundColor(.green) modifier.
  
  
## Section 3
**Combine Views Using Stacks**

  Beyond the title view you created in the previous section, you'll add text views to contain details about the landmark, such as the name of the park and state it's in.
  
  When creating a SwiftUI view, you describe its content, layout, and behavior in the view's body property; however, the boy property only returns a single view. You can combine and embed multiple views in _stacks_, which group views together horizontally, vertically, or back-to-front.
  
  In this section, you'll use a vertical stack to place the title above a horizontal stack that contains details about the park.
  
  You can use Xcode's structured editing support to embed a view in a container view, open an inspector, or help with other useful changes.
  
### Step 1
  Command-click the text view's initializer to show the structured editing popover, and then choose **Embed in VStack**.
  
  Next, you'll add a text view to the stack by dragging a Text view from the library.
  
### step 2
  Open the library by clicking the plus button (+) at the top-right of the Xcode window, and then drag a Text view to the place in your code immediately after the "Turtle Rock" text view.
  
### Step 3
  Replace the Text view's placeholder text with **Joshua Tree National Park**.
  
  Customize the location to match the desired layout.
  
### Step 4
  Set the location's font to subheadline.
  
### Step 5
  Edit the VStack initializer to align the views by their leading edges.
  
  By default, stacks center their contents along their axis and provide context-appropriate spacing.
  
  Next, you'll add another text view to the right of the location, this for the park's state.
  
### Step 6
  In the canvas, Command-click **Joshua Tree National Park**, and choose **Embed in HStack**.
  
### Step 7
  Add a new text view after the location, change the placeholder text to the park's state, and then set its font to subheadline.
  
### Step 8
  To direct the layout to use the full width of the device, separate the park and the state by adding a Spacer to the horizontal stack holding the two text views.
  
  A _spacer_ expands to make its containing view use all of the space of its parent view, instead of having its size defined only by its contents.
  
### Step 9
 Finally, use the padding() modifier method to give the landmark's name and details a little more space.
 

## Section 4
**Create a Custom Image View**
  

