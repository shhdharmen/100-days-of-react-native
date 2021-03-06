# 100-days-of-react-native with WhiteBoard

This project serves as logs entries for the original react native project called [WhiteBoard](https://github.com/shhdharmen/WhiteBoard). I started this project on _10th October, 2019_.

The project can be viewed at:

| View                   | URL                                                                                                  |
| ---------------------- | ---------------------------------------------------------------------------------------------------- |
| Frontend Git :octocat: | [https://github.com/shhdharmen/WhiteBoard](https://github.com/shhdharmen/WhiteBoard)                 |
| Expo view :iphone:     | [https://expo.io/@shhdharmen/WhiteBoard](https://expo.io/@shhdharmen/WhiteBoard)                     |
| ---------------------- | ------------------------------------------------------------------------------------                 |
| Backend Git :octocat:  | [https://github.com/shhdharmen/white-board-strapi](https://github.com/shhdharmen/white-board-strapi) |

I am planning to build something with these [requirements](REQUIREMENTS.md).

## Logs

<!--

### Day 0: February 30, 2016 (Example 1)

#### (delete me or comment me out)

**Today's Progress:**

Fixed CSS, worked on canvas functionality for the app.

**Thoughts:**

I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link to work:**

[Calculator App](http://www.example.com)

---

-->

### Day 0: October 10-11, 2019

#### :white_check_mark: Initial setup done

**Today's Progress:**

- Read getting started docs for [React Native](https://facebook.github.io/react-native/docs/getting-started) and [Expo](https://docs.expo.io/versions/latest/).
- Created main project using [Expo's Managed Workflow](https://docs.expo.io/versions/v35.0.0/workflow/exploring-managed-workflow/) with Typescript.
- Created both repos, logs and main project.
- Setup github actions to deploy and publish in main project.

**Thoughts:**

- It took some more time to complete initial setup, but that's okay. I am happy with it :smile:.

**Links to work:**

| Link                                     | URL                                                                                                              |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Logs Project Github Pages :octclipboard: | [https://shhdharmen.github.io/100-days-of-react-native/](https://shhdharmen.github.io/100-days-of-react-native/) |
| Main Project Git :octocat:               | [https://github.com/shhdharmen/WhiteBoard](https://github.com/shhdharmen/WhiteBoard)                             |
| Web :computer:                           | [https://shhdharmen.github.io/WhiteBoard/](https://shhdharmen.github.io/WhiteBoard/)                             |
| Expo :iphone:                            | [https://expo.io/@shhdharmen/WhiteBoard](https://expo.io/@shhdharmen/WhiteBoard)                                 |

---

### Day 1: October 12, 2019

#### Server and API setup

**Today's Progress:**

- Created api server [White Board Strapi](https://github.com/shhdharmen/white-board-strapi) project using [Strapi](strapi.io)
  - Created 4 content-types in it:
    - Notes
    - Categories
    - Colors
    - Tags
- Also deployed it on heroku

**Link to work:**

[White Board Strapi Repo](https://github.com/shhdharmen/white-board-strapi)

---

### Day 2/3: October 14/15, 2019

#### Further authentication setup on server

**Today's Progress:**

- I've setup [policies](https://strapi.io/documentation/3.0.0-beta.x/concepts/policies.html#concept) so that logged-in user can see only owned notes, categories, tags.
- Added [native base](https://nativebase.io/) for UI kit, [lottie](https://airbnb.io/lottie/#/) for loader animation and [react navigation](https://reactnavigation.org/en/) for routing.
- Changed `primary` theme color of native base, guide [here](https://docs.nativebase.io/Customize.html#theaming-nb-headref).
- Created a `Main` component, which will hold all the navigations like below:
  - `HomeScreen` - Currently it's showing only loader. I will logically hide it and show dashboard page if logged in and login page if not.
  - `DashboardScreen` - Just a skeleton
  - `LoginScreen` - Just a skeleton
  - `RegisterScreen` - Just a skeleton
  - `ForgotPasswordScreen` - Just a skeleton

**Thoughts:**

- I will continue on how to store `jwt` token in react native and will implement login, register and forgot password next.

**Link to work:**

- [Backend commit for user authentication](https://github.com/shhdharmen/white-board-strapi/commit/63868495d0917dff9117e9d6e03ac7bc1e62a48b)
- [Frontend commit: added native base, lottie, react navigation](https://github.com/shhdharmen/WhiteBoard/commit/0c9a5aa589f1c1e163d1cf5af414b2f16fd4159a)

---

### Day 4-5: October 18-19, 2019

#### Login, Auth flow and jwt token management

**Today's Progress:**

- Upgraded `expo-cli` version
- Read [Authentication flows](https://reactnavigation.org/docs/en/auth-flow.html) for React Navigation.
- Created [animated routes](https://reactnavigation.org/docs/en/animated-switch-navigator.html).
- Read about [environments](https://github.com/luggit/react-native-config/issues/249#issuecomment-386090809) and implemented.
- Used [axios](https://github.com/axios/axios) for HTTP client.
- Implemented show/hide for password field.

**Link to work:**

- [Commit link](https://github.com/shhdharmen/WhiteBoard/commit/af7217c7e67f1bb412b7ebf0382f8ea2a9de5390)

---

### Day 6: October 31, 2019

#### Fetch notes

**Today's Progress:**

- Fixed login UI.
- Fetched notes after login.
- Used `Card` of NativeBase to preview notes.
- Added header in login and home screen.
- Added fonts: `Poppins` and `AnonymousPro`, thanks to [https://fontpair.co/](https://fontpair.co/).

**Link to work:**

[fonts, fetch notes, login ui corrections](https://github.com/shhdharmen/WhiteBoard/commit/e86de5b25995953f161f670585eca0758866f251)

---

### Day 7: November 1, 2019

#### Change in content types, add note ui, settings ui, no notes ui

**Today's Progress:**

- Created couple of UIs - No notes UI, Add Note UI, Settings UI.
- Added animations using [react-native-animatable](https://www.npmjs.com/package/react-native-animatable).
- Changed content types on backend and removed relationships.
- Added [list-is-empty](https://icons8.com/ouch/illustration/mirage-list-is-empty) image when no notes are there.
- Created some shared components: `HeaderText` (and input), `TextLoader` to handle custom stylings.

**Thoughts:**

I really struggled with animations, but [react-native-animatable](https://www.npmjs.com/package/react-native-animatable) made it easier at last.

---

### Day 8: November 23, 2019

#### Colors, Archive, Edit and Delete Note

**Today's Progress:**

- Used `react-native-color-palette` for color selections
- Added update api calls
- Showing delete confirm dialog before actually deleting
- Archive note and undo it (by toast button)

---

### Day 9: December 10th, 2019

**Today's Progress:**

Fixed iOS specific issue. TouchableNativeFeedback is only working in android. So, made a shared component which will return TouchableNativeFeedback for android and TouchableHighlight for iOS.

**Link to work:**

[Commit](https://github.com/shhdharmen/WhiteBoard/commit/a3dda4eb463d7743018af51223073f33bead63a4)

---

### Day 10: December 11th, 2019

**Today's Progress:**

Added a searchbar with menu, search and thumb icons.

**Link to work:**

[Commit](https://github.com/shhdharmen/WhiteBoard/commit/8b8f06f5327a0b349bb5215ffbc79f006bc1db50)

---