# User Testing
## Functionalities Tested
- **Sign up/log in:** Users can create an account with Name, Username, and Password then log in with those credentials
  - [frontend/src/pages/Login.tsx](https://www.google.com/url?q=https://github.com/UWSocialComputing/power-hour-code/blob/main/frontend/src/pages/Login.tsx&sa=D&source=editors&ust=1685776897285883&usg=AOvVaw1-dQe1HX7JlWc5_m6_D5GG)
  - [frontend/src/pages/Signup.tsx](https://www.google.com/url?q=https://github.com/UWSocialComputing/power-hour-code/blob/main/frontend/src/pages/Signup.tsx&sa=D&source=editors&ust=1685776897286498&usg=AOvVaw0WnCoWjuJjB1PtwtogfC6V)
- **Join/leave queue:** Users can click the “Join Queue” button allowing them to fill out a form with basic information (name, question type, question details, in-person/online, and if they’re willing to collaborat). They can also leave if they choose to.
  - [frontend/src/pages/Home.tsx](https://www.google.com/url?q=https://github.com/UWSocialComputing/power-hour-code/blob/main/frontend/src/pages/Home.tsx&sa=D&source=editors&ust=1685776897287362&usg=AOvVaw2J3-gExytA1gyToAeKsTx6)
- **Chat:** Users can chat with other users by creating groups. For testing , the user is instructed to add a specific user to a group and we would respond to their messages.
  - [frontend/src/pages/Home.tsx](https://www.google.com/url?q=https://github.com/UWSocialComputing/power-hour-code/blob/main/frontend/src/pages/Home.tsx&sa=D&source=editors&ust=1685776897288072&usg=AOvVaw2myR1UnrzrdotPAEKdQ7l7)
  - [frontend/src/pages/objects/CreateChatView.tsx](https://www.google.com/url?q=https://github.com/UWSocialComputing/power-hour-code/blob/main/frontend/src/pages/objects/CreateChatView.tsx&sa=D&source=editors&ust=1685776897288539&usg=AOvVaw0a1sLinFiBjPfqhQM-I_wG)
- We omitted the TA flow and kudos system for now, and we have pre-populated notifications displayed.

## Screenshots

|     Log in  |    Queue     |
|     :--:    |     :--:    |
| ![Login](/power-hour/img/UserTestingLogin.png){: height="250px" width="400px" }|![Queue](/power-hour/img/UserTestingQueue.png){: height="250px" width="400px" }|

|     Join queue form  |   Queue joined      |
|     :--:    |     :--:    |
| ![Queue form](/power-hour/img/UserTestingQueueForm.png){: height="250px" width="400px" } | ![Queue joined](/power-hour/img/UserTestingQueueJoined.png){: height="250px" width="400px" } |

|     Collaborate   |     Chat    |
|     :--:    |        :--:       |
| ![Collaborate](/power-hour/img/UserTestingCollaborate.png){: height="250px" width="400px" } | ![Chat](/power-hour/img/UserTestingChat.png){: height="250px" width="400px" } |

## User Testing Findings

We conducted user testing with 4 students and overall received positive feedback on the overall flow of the queuing system.
- **Account creation/login:** Students could successfully create an account with a username and password. Some participants thought this was connected to the UW NetID system and tried to use their existing credentials to log in. We plan to add a note to clarify that the systems are separate. Users also mentioned that it would be easier if they could be directly logged into the system after creating an account instead of logging in again.
- **Queuing table:** Students could easily understand each column of the table. They looked for students working on the same question and were open to collaborating. They thought the colors of the Status and Open to Collaborate columns made sense. They also recognize the Collaborate buttons as clickable.
- **Join queue form:** Students thought the form had an appropriate number of questions and was short enough to not discourage people from joining office hours.
- **1-1 collaboration:** After identifying the student they wanted to collaborate with, they clicked on the green Collaborate button to open a chat room as expected. One participant was confused on how a student could be in-progress (working with a TA) but still be open to collaborate. They mainly used the chat to ask if the other student wanted to work together or where they were seated physically if they were listed as “In-Person” on the queue. Participants noted that for some classes it wouldn’t make sense to collaborate over a text chat so they would have to make a separate Zoom link which would be a hassle.
- **1-many collaboration:** Currently, users can add multiple members when starting a group chat but they can’t add members to an existing group chat. When we asked students to collaborate with different people, they tried to click the group icon to add more members. It was also unclear that they could click the “Collaborate” button again to make a new chat group. When making a new group chat, users didn’t know they could select more than one student on the dropdown and suggested we use a checkbox or plus/minus icons next to the user names to indicate multi-selection.
- **Active Sessions:** One participant thought that active sessions meant the number of times they have visited the TA this quarter. By the end of the test, they realized it was the number of group chats they were in. They suggested that the Active Sessions box was unnecessary. Overall, there was some confusion on the meaning of “session” so we plan to change this to “group chat”.
- **Notifications:** We haven’t fully implemented a notifications feature but asked for feedback on what students would like to see. They expected notifications if they were next in line in the queue or if a student had invited them to a group chat. They also suggested push notifications would be helpful because they’re often switching between tabs while waiting in office hours.

Overall, many of the functionalities like joining the queue and chatting with other students work as intended. Users were able to navigate through most all functionalities smoothly and thought this system was well organized and would improve their office hours experience.

## Upcoming Changes
- **Notifications:** As suggested by participants, we will notify students if they are next in the queue and if a student has added them to a group chat. We also plan to add browser push notifications as a stretch goal
- **1-many collaboration:** We will continue iterating on this user flow by allowing users to add people to existing group chats and add checkmarks to the drop down when creating a new group.