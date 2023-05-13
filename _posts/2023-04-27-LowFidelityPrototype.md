# Low-Fidelity Prototype

Our prototype includes the following components:
- **The OH queue**: The OH queue should include information on what students are working on. We use a spreadsheet to simulate it so we can learn what information users need on the queue interface.
- **Joining the OH**: When joining the queue, students will need to enter some information before getting help. We use a google form that asks for students’ name, question type, details on their question, and whether or not they are open to collaboration.
After submitting, we will show them a spreadsheet that we will populate with their response and additional columns such as timestamp and status. This will allow them to track their place in the queue and see what other students are working on, as well as their willingness to collaborate.
- **Student collaboration**: There should also be a built-in communication tool that allows students to connect and collaborate with each other in the form of a chat. To simulate that, we have a google chat open to the right of the queue spreadsheet allowing students to create or join a Space and chat with other students who indicated “Yes” to Open to Collaborate. We will create the space for them once they tell us who they want to include in the new collaboration session.
We will join separately to act as the other students, as well as an automated message that reminds students about collaboration policy and notifying students when they are next in the queue.

## Prototype screenshots
Main interface with queue and collaboration chat side by side:
![main interface prototype](/power-hour/img/PrototypeMainInterface.png)
Users can switch to all students' views to see all active students in OH session. Some of them can be helped or idle (not needing help from the TA at the moment) but still open to collaboration.

Google form for providing information to join OH:
![form prototype](/power-hour/img/PrototypeForm.png)

Chat interface with collaboration policy message from the bot:
![chat prototype](/power-hour/img/PrototypeChat.png)

## Findings

Our goal with this session was to understand how users would interact with our solutions and make improvements to the user flow. Overall, participants liked the idea of a new office hours queuing and collaboration system. Features like the OH estimation time, kudos, and chat rooms for collaboration were well received. We will be moving ahead with the project because the students and TAs we interviewed used the features mostly as intended and saw how this solution would address problems they face in office hours.

## Elements to keep
- **Kudos:** Participants liked the ability to give and receive Kudos. They felt appreciated when other students gave kudos to them and thought it effectively fosters collaboration. We will extend this feature by allowing TAs to also give kudos.
- **Spreadsheet columns:** Participants liked that they were able to see what question other students were working on and their status as it helped them determine who to collaborate with. The timestamp also gave them reassurance that everyone is in the right place of the queue.
- **Chat rooms:** Participants liked that the chat room was side-by-side with the queue because it was easy to collaborate while tracking their place. They also liked that they could add specific students to a group chat.
- **Option to leave the queue and estimated wait time in queue:** Both of these queue management features were strongly recommended by participants as it allowed for better understanding and management of the queue from both students and TAs.

## Elements to revise
- **Collaboration indicator:** Even though participants were willing to collaborate with others, many were concerned that if they indicated that they were willing to collaborate with others, TAs would deprioritize them in the queue. We will add a note in the office hours form that this will not affect their priority. We will also need to add a location indicator for potential hybrid office hours.
- **Joining the queue:** Some participants thought that they were supposed to edit the spreadsheet directly instead of clicking “Join queue”. We plan to either change the flow so that the form to join the queue is first or add a pop-up modal to the queue.
- **Adding a "getting started" question type:** This was a suggestion mentioned by multiple participants as one of the common types of questions students come into office hours with.
- **Wait-time estimation:** Participants did not trust that the estimate would be accurate because it’s dependent on the student and question difficulty. Our current estimates are based on the question type (selected by students on the form) and the number of students in line. While we are also struggling to make this more accurate, one way might be to add a timer or banner at 10-15 minute intervals to remind students that their time is up. Our calculations would be based on those intervals.
- **Removing entries of those who have left or logged out:** This will help TAs manage who is still left in the queue, and remove students who have logged out.
- **Queuing form:** Participants thought that some questions on the form felt redundant or too much information. We plan on removing the “What specifically do you need help with” question or make this data only visible to TAs.

## Great suggestions that are lower priority:
- Whiteboard/drawing feature in the chatroom
- Customizable queuing form where TAs or professors can edit and add their own questions and answer fields
