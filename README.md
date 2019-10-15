# 100-days-of-react-native with WhiteBoard

This project serves as logs entries for the original react native project called [WhiteBoard](https://github.com/shhdharmen/WhiteBoard). I started this project on _10th October, 2019_.

The project can be viewed at:

| View                   | URL                                                                                                  |
| ---------------------- | ---------------------------------------------------------------------------------------------------- |
| Frontend Git :octocat: | [https://github.com/shhdharmen/WhiteBoard](https://github.com/shhdharmen/WhiteBoard)                 |
| Web view :computer:    | [https://shhdharmen.github.io/WhiteBoard/](https://shhdharmen.github.io/WhiteBoard/)                 |
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
