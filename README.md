## Demo iOS App

## How to make a basic iOS app in 20 minutes

### Requirements

- An Apple laptop with the latest version of OSX installed or a virtual machine with the same on a Windows machine.
	- ** Please note virtual machines will likely suffer performance drops
- An active internet connetion to install Xcode and/or other software
- The latest version of Xcode

### Skill level

- Beginner, no prior programming experience necessary 😄

### Setting things up

- Download Xcode from the [Mac App Store](https://itunes.apple.com/us/app/xcode/id497799835?mt=12). 
	- It can take roughly an hour to download and install
- Open Xcode
	- Select `Create a new Xcode project`
		- Make sure `iOS` is selected and `Single View App` is selected in the main menu
		- Click `Next`
		- Name your project `iOS Demo - changing text color buttons`
		- Under `Orgranization Identifier` put `ios-demo-buttons_and_colors`
		- Leave all other areas as default
		- Click `Next`
		- Click `Finish`
		- In the window that pops up, click `New Folder` and name it `iOS Demo`
		- Click `Create`
- Testing your project
	- Start by running your project, we just want to make everything is working 👍🏻
	- 🎬  You can do that by clicking the ▶️ at the top of the window within Xcode, or by clicking `⌘ + r` on your keyboard
	- Once you've done that, a window should open with an emulator of an iPhone, mine is an iPhone XR which we'll be using for this demo

### Create the app components 

- On the left-hand side, near the toolbar, click the `Main.storyboard` file
	- Reference, screenshot <img width="2002" alt="1" src="https://user-images.githubusercontent.com/17191728/58447622-d86f7900-80b9-11e9-8cf2-d8874db20225.png">
- 👁 You should now see a screen with a blank iPhone outlined
- Click the 🔘 icon which looks like an old iPhone 5 home button at the right-most area of the screen
	- Reference, screenshot <img width="2002" alt="2" src="https://user-images.githubusercontent.com/17191728/58447623-d9080f80-80b9-11e9-97d0-abd12c51f42e.png">
	- A menu should open
		- type in `view` and drag `Text View` to the blank iPhone canvas
		- type in `text` and drag `Text Field` to the blank iPhone canvas
		- type in `button` and drag `Button` to the blank iPhone canvas
- 👁 On your blank iPhone canvas you should have all three elements listed below
- Position each element such that the `Text View` is above the `Text Field` and the `Button` is to the right of the `Text Field` -> please note exact positioning is not 100% necessary
	- Reference, screenshot <img width="2002" alt="3" src="https://user-images.githubusercontent.com/17191728/58447624-d9080f80-80b9-11e9-8945-83341495ce2e.png">
- 🎬 Re-run your app to make sure it's working so far - check the `Don't ask me again` box
	- You should now see all your elements in the app on the emulator and be able to enter text in the `Text Field`
	- Reference, screenshot 
	<img width="584" alt="4" src="https://user-images.githubusercontent.com/17191728/58447625-d9080f80-80b9-11e9-813b-b374c8db0b33.png">
	
### Create the app logic

- Click on the double-circle icon at the top right-most part of the screen near where the home button icon was before
	- 👁 You should now see a second window open next to your iPhone canvas that has some code in it
		- Reference, screenshot <img width="1920" alt="5" src="https://user-images.githubusercontent.com/17191728/58447626-d9080f80-80b9-11e9-8d7a-d2201651c497.png">
	- Now click on `Text Field` in the toolbar to the left and click `control` while dragging your mouse to line 19 in the window next to your iPhone canvas
		- Reference, screenshot <img width="1920" alt="6" src="https://user-images.githubusercontent.com/17191728/58447627-d9080f80-80b9-11e9-8d78-423306c88e48.png">
		- Name it `text_field` and make sure `Outlet` is selected instead of `Action` just above the name field
		- Do the same thing for the `Text View` component but name it `text_view`
		- Do the same thing again for the `Button` component but name it `button` and make sure to select `Action` this time instead of `Outlet`
	- 👁 In the window to the right of your iPhone canvas you should now see two IBOutlets, 1 for your `text_view` and 1 for your `text_field`, followed by an IBAction for your button
		- Reference, screenshot <img width="1920" alt="7" src="https://user-images.githubusercontent.com/17191728/58447628-d9080f80-80b9-11e9-8774-17e03d62f886.png">
	- Enter the below line of code in between the *curly braces* `{}` for the IBAction component reference to your button:
		- `text_view.text = text_field.text`
		- 🎬 run your app to test your code
		- Reference, screenshot <img width="1920" alt="8" src="https://user-images.githubusercontent.com/17191728/58447629-d9a0a600-80b9-11e9-8a3c-14127406e53d.png">
- 🧪 Let's test the code we have written:
	- Enter your name in the `text_field` component and click the button next to it
	- 👁 you should now see the name you entered in the `text_field` appear in the `text_view` component, yay!
		- Reference, screenshot
		<img width="584" alt="9" src="https://user-images.githubusercontent.com/17191728/58448711-744eb400-80bd-11e9-8529-3591b41bc783.png">

### Demo

- View basic demo on [YouTube](https://youtu.be/DX73JKDFE3k)
- View advanced demo on [YouTube](https://youtu.be/NrLSqDgjyMk)

### Concluding thoughts

Creating an iOS app is fun and easy! My hope is that you were able to create your own iOS app today and that you enjoyed doing so. I'll document this demo on GitHub if you'd like to reference it in the future, feel free to share it with your friends and family.
