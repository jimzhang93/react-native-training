# React Native training

## Initial set up

-brew install watchman

-brew install flow (static type checker for JS)

-Ensure Xcode version of 7 or higher (https://developer.apple.com/xcode/downloads/)

-We will be only doing iOS today. For Android, you must download the Android SDK and JDK (Java Development Kit) and install an emulator (genymotion or default).

-Install the React Native CLI (npm install -g react-native-cli)

-Initialize our example app (react-native init react-native-training)

Now, we have a React Native app initialized. At this point, we can initialize the iOS simulator that comes with Xcode or set up the Android environment and initialize the simulator there.

However, mosaic mobile started with the Ignite boilerplate and that is the industry standard when starting a new mobile app due to its comprehensiveness. (https://github.com/infinitered/ignite)


## What is React Native?

-It is the React we have come to know and love written in good old JavaScript.

-It was created by Facebook in 2015 to solve a lingering problem that developers often complained about - how to create heavy and scalable apps in iOS and Android in a concurrent fashion.

-Mobile development was starting to take center stage and developing apps for different operating systems proved to be extremely tedious.

-Developers realized that virtual DOM feature of React allows for content to be rendered to targets other than browsers

-Output is rendered in Java or Objective-C, depending on the target OS

-Allows for platform specific UI components, such as pickers and navigation routers

-Actions consist of swiping, touching, scrolling, and dragging on mobile screens

-Slogan is 'learn once, write anywhere'

## Demo with familiar app

For this demo, we will use mosaic mobile to demonstrate a few basic concepts.

-Clone the repo here (https://github.com/simplefractal/mosaic-mobile)

-npm install

-Make sure to pull start the mosaic backend (mosaic-rails-api on the master branch)

-Go to dev branch in mosaic-mobile and make sure it is up to date, and then branch off to another branch called 'training'

-Open another tab in mosaic-mobile and npm start

-react-native run-ios

## Things I found challenging when learning RN

-Different components (view vs div), a list can be found at https://facebook.github.io/react-native/docs/components-and-apis.html

-Different styling (Javascript objects vs CSS)

-Lack of live reload and long feedback cycle (hot reload often does not work)

-Modal logic handling (in screens with as many as 20 modals, state must be managed by the parent screen container because stacking modals erase the state of modals beneath them)

-Transition animations (when switching into different pages)

-E2E testing with Cavy

-Getting multiple features to work in conjunction (such as drag/droppable and swipeable rows)

-Timing when switching screens and loading data (setTimeout is very handy in RN development) for a seamless experience - such as DOM unable to target list when switching to a new view when the list has not loaded yet

-Lack of documentation since RN is so young

-Lack of third party components for certain features for same reason



-App architecture overview

-Styling

-Talk about challenges in the app, if time permits
