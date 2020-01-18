# Creating and Combining Views
  This tutorial guides you through building _Landmarks_ -- an iOS app for discovering and sharing the places you love. You'll start by building the view that shows a landmark's details.

  To lay out the views, Landmarks uses stacks to combine and layer the image and text view components. To add a map to the view, you'll include a standard MapKit component. As you refine the view's design, Xcode provides real-time feedback so you can see how those changes translate into code.

  Download the project files to begin building this project, and follow the steps below.

## section 1
### Create a New Project and Explore the Canvas
  Create a new Xcode project that uses SwiftUI. Explore the canvas, previews, and the SwiftUI template code.

  To preview and interact with views from the canvas in Xcode, ensure your Mac is running macOS Catalina 10.15.

  
#### Step 1
  Open Xcode and either click **Create a new Xcode project** in Xcode's startup window, or choose **File > New > Project.**

#### Step 2
  In the template selector, select **iOS** as the platform, select the **Single View App** template, and then click **Next.**

#### Step 3
  Enter "Landmarks" as the Product Name, select **SwiftUI**for the user interface, and click **Next**. Choose a location to save the landmarks project on your Mac.

#### Step 4
  In the Project navigator, select ContentView.swift.

  By default, SwiftUI view files declare two structures. The first structure conforms to the View protocol and describes the view's content and layout. The second structure declares a preview for that view.

#### Step 5
  In the canvas, click **Resume** to display the preview.

  **Tip**
  If the canvas isn't visible, select **Editor > Editor and Canvas** to show it.

  

