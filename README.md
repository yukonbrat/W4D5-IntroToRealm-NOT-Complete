# W4D5-IntroToRealm-NOT-Complete

<h2>Intro to Realm</h2>

<p>Once you are comfortable with CoreData, you can try using to Realm to persist data. Realm is an open-source alternative to CoreData, it has a native iOS and Android SDK, and is also a bit more user-friendly.</p>

<h2>Installing CocoaPods and Realm</h2>

<p>First of all let’s install Realm. To do that, we are going to use CocoaPods to helps us do that. CocoaPods is a dependency manager and allow us to easily add third party code into our projects.</p>

<p>Before CocoaPods we had to download files we wanted to use and import it into our project. Now we can use CocoaPods and if helps us in the following way:
    - Makes adding files to our projects easier
    - Makes managing updates for those added files easier (we just use the command &quot;pod install&quot; and it downloads and links the new files)</p>

<ul>
<li><p>First of all, follow the instructions on <a href="https://cocoapods.org/" target="_blank">https://cocoapods.org/</a> to install cocoapods</p></li>
<li><p>We are going to add Realm to this project. Firstly, add a file called: Podfile</p></li>
<li><p>Inside this file add the below text:</p></li>
</ul>

<p>use_frameworks!</p>

<p>pod &#39;Realm&#39;</p>

<ul>
<li><p>This adds Realm, and the use_frameworks! adds the library as a framework and even enables Swift support (if needed).</p></li>
<li><p>Now run the command &quot;pod install&quot;</p></li>
<li><p>Once you start using third party libraries with cocoapods, you must use the .xcworkspace file instead of the .xcodeproj file going forward.</p></li>
</ul>

<p>You&#39;ve added Realm and you can start the assignment.</p>

<p>Be sure to download the Realm browser from the Mac App Store. It will allow you to see what you have saved in Realm, and is great for debugging.</p>

<h3>Objective</h3>

<p>We are going to make a Furniture Tracker. We are going to track all the rooms in a house and track all the furniture items in a room.</p>

<h3>Steps</h3>

<ul>
<li><p>Start off with a Master-Detail template, make sure to switch Core Data off</p></li>
<li><p>Make 2 RLMObjects. Room + Furniture</p></li>
<li><p>When you click on the + Button on the Root View Controller, you can add a Room. Use a UIAlertController with a textField</p></li>
<li><p>When you click on a specific room, you segue into another Table View Controller. Add a + Button which can add furniture items. Use a UIAlertController with a textField. This viewController should also query all furniture items for a specific room.</p></li>
</ul>

<p>Congrats, you are now ready to use Realm for Rotten Mangoes and others apps for which you would like to persist data!</p>
