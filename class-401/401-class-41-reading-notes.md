# React Native

[getting started with react native](https://reactnative.dev/docs/intro-react)

- Name three Core Components of React Native and describe what they do.
  - \<View>: A container that supports layout with flexbox, style, some touch handling, and accessibility controls
  - \<Text>: Displays, styles, and nests strings of text and even handles touch events
  - \<Image>: Displays different types of images
- What problem does React Native solve (why call it native)?
  - React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code.
- What are the building blocks of a React Native app? How does that compare to a React app?
  - Components, JSX, props, state

[expo](https://docs.expo.dev/tutorial/introd)

- What solution does expo provide?
  -'Build one project that runs natively on all your users' devices'
- Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.
  - Managed
- What is the difference between React Native and Expo?
  - When you write code in Expo you are writing React Native code. Expo is a set of tools built on top of React Native. [source](https://stackoverflow.com/questions/39170622/what-is-the-difference-between-expo-and-react-native)

[expo snack](https://snack.expo.dev/)

- Checkout this tool. What does snack allow you to do?
  - Expo Snack is an open-source platform for running React Native apps in the browser. It dynamically bundles and compiles code and runs it in the Expo Client or in a web-player. Code can be saved as "Snacks" and easily shared with others.

[ejecting](https://docs.expo.dev/expokit/eject/?redirected)

- What does “eject” mean within the context of Expo?
  - Expo allows you to eject your pure-JS project from the Expo iOS/Android clients, providing you with native projects that can be opened and built with Xcode and Android Studio. Those projects will have dependencies on ExpoKit, so everything you already built will keep working as it did before.
- When should you not eject?
  - All you need is to distribute your app in the iTunes Store or Google Play. Expo can build binaries for you in that case. If you eject, we can't automatically build for you any more.
  - You are uncomfortable writing native code. Ejected apps will require you to manage Xcode and Android Studio projects.
  - You enjoy the painless React Native upgrades that come with Expo. After your app is ejected, breaking changes in React Native will affect your project differently, and you may need to figure them out for your particular situation.
  - You require Expo's push notification services. After ejecting, since Expo no longer manages your push credentials, you'll need to manage your own push notification pipeline.
  - You rely on asking for help in the Expo community. In your native Xcode and Android Studio projects, you may encounter questions which are no longer within the realm of Expo.
- Why might you choose to eject?
  - Your Expo project needs a native module that Expo doesn't currently support. We're always expanding the Expo SDK, so we hope this is never the case. But it happens, especially if your app has very specific and uncommon native demands.

## Tutorial

[react native basics](https://reactnative.dev/docs/tutorial)

## Bookmark and Review

[react native](https://reactnative.dev/)

## Additional Questions

- Looking ahead at this module’s course schedule, What do you look forward to learning?
  - React Native & Expo
- What are your learning goals after reading and reviewing the class README?
  - To understand React Native and to use it to build out a functioning application

[Return home](https://khofstetter94.github.io/reading-notes/)
