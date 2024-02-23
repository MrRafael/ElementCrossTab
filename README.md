# Element Cross Tab

### This is a test with WebSocket

![tabs-2](https://github.com/MrRafael/ElementCrossTab/assets/19240037/817de62e-5098-41ea-bdbb-8a376a17d5aa)



Its creates the illusion of the element disappears in one tab and appears in another tab, but the element its present in all open tabs, just not visible because the the element is oriented to the screen size/position and not to the browser window, also there is the property in css ```overflow: hidden;``` to not allow scrolling and finding the element.
It's possible to move the window 'to find' the element, if the window is small than the screen, and you move the element 'out of the window'. it's possible to move the window to the element direction to see the element again, to allow this behavior I created a ```setInterval(correctPosition, 4)``` its take the differences between the window position and 0,0 of the screen, the setInterval was used because there is now event that triggers when the window moves. With this approach it should create an illusion that the element remains stopped when the window moves, but even with an interval of 4ms it's not fast enough to create this illusion, maybe because the time the DOM takes to update.

### Pre-requisites
Before you begin, you will need to have the following tools installed on your machine:
[Git](https://git-scm.com), [Node.js](https://nodejs.org/en/).
In addition, it is good to have an editor to work with the code like [VSCode](https://code.visualstudio.com/)

#### 🎲 Running

```bash

# Clone this repository
$ git clone https://github.com/MrRafael/ElementCrossTab.git

# Go to the floder
$ cd ElementCrossTab

# install depencies
$ npm install

# Run the server
$ node index.js

#  go http://localhost:3000 

```
---

#### :video_game: Controll the red ball
Use W,A,S,D to move the ball, W to Up, A to Left, S to Down, D to Right.
![4617690](https://github.com/MrRafael/ElementCrossTab/assets/19240037/7ba5f396-23e5-4978-9aab-baa3c10c3570)


<h3 id="tech-stack"> 🛠 Tech Stack </h3>

The following tools were used in the construction of the project:

-   **[Expo](https://expo.io/)**
-   **[Socket.IO](https://socket.io/)**
-   **[Express](https://expressjs.com/)**
