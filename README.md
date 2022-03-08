## GearWheelAndSettings
This is a sample solution to demonstrate the issue of display of Image depending on the Image's source filename. The issue is:
* If the image file name is *'icon_gear_wheel.png'* the image is not displayed either as a **ToolbarItem** or as an **Image**.
* If the image file name is *'icon_settings.png'* then the image will be displayed.

I noticed this first as I set the *'icon_gear_wheel.png'* as the **IconImageSource** of a **ToolbarItem** in 6th Tab of a **TabbedPage** in iOS. Then this issue was not observed in Android.
But now after I could resolve the issue in iOS after renaming the icon file names to ***'icon_settings...png'*** in iOS Resources, I noticed the same issue in Android too with the latest update to Xamarin.Forms.

This solution demonstrates this issue in both Android and iOS right in the first page of a TabbedPage. This issue was found in Xamarin.Forms versions ***5.0.0.2196*** and ***5.0.0.2337***.
