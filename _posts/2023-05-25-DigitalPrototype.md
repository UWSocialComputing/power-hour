# Digital Prototype
## Problem
In many CS classes at UW, there are hundreds of students and only a handful of TAs. This leads to a bottleneck in office hours where students end up waiting anywhere from 10 minutes to an hour to speak with the TA. They join the queue by writing their name on a whiteboard or Zoom chat and struggle with the assignment alone until they can speak with the TA. While researching the pain points in office hours, we saw how much time students had to waste waiting in line. We wanted to build a solution that helps students leverage this time to collaborate with others and solve smaller problems on their own. This would ultimately reduce the time that each student needs with the TA and make office hours more efficient.

## Solution
### Feature Overview
With the goal of fostering collaboration and productivity, we developed 5 main features:
1. **Queuing form:** Students enter basic information about their question, whether they’re in-person or online, and if they’re open to collaborating with other students during the office hours period. The form can be edited after submission.

    ![Queuing form](/power-hour/img/DigitalPrototypeForm.png)

    *Design notes - When testing our low-fidelity prototype, we found that long, full-page forms overwhelmed users and discouraged them from entering the queue so we paired the form down to a modal with only 4 short questions.*
2. **Queuing table:** The form data populates a queuing table that all students in the office hour session can view. The Timestamp and Status columns are automatically populated. Students can click Collaborate in the Open to Collaboration column to message other students in line.

   ![Queue](/power-hour/img/DigitalPrototypeQueue.png)

    *Design notes - User testing participants didn’t know that Collaborate in the Open to Collaboration column was a button so we added a shadow on hover.*
3. **Chat rooms:** Students can create a group and message each other while waiting in the queue. They can text or simply react to messages with an emoji. Users can add people to the group chat by selecting their name in the drop down. There is also an automated bot message reminding members on the course collaboration policy.

    ![Collaborate](/power-hour/img/DigitalPrototypeCollaborate.png)

    ![Chat](/power-hour/img/DigitalPrototypeChat.png)

    *Design notes - In an earlier iteration, our users didn’t know that they could add multiple people to a group chat due to dropdown design so they suggested we add checkboxes. We also added the ability for the admin or the creator of the group chat to add additional members to the chat.*
4. **Wait-time estimate:** The system estimates the time it will take for the student to reach the front of the queue by taking historic wait-time averages per question type multiplied by the number of that question type currently in the queue.

   ![Chat](/power-hour/img/DigitalPrototypeWait.png)

   *Design note - The wait-time card changes color based on the estimated wait-time.*

5. **Notifications:** Students receive a bell notification if they’ve been added to a group chat and a banner if they’re near the front of the queue.

    ![Bell notification](/power-hour/img/DigitalPrototypeBell.png)

    ![Banner notification](/power-hour/img/DigitalPrototypeBanner.png)

    *Design note - When the estimated wait time is less than 10 minutes students will see a banner across the page asking them to get ready for interacting with the TA.*

## Technical Overview

We used Firebase for database management and Azure to host the backend server. We used Flask to create API endpoints to collect and send queue data from the database to the frontend and synchronize user data between the Stream Chat API and our own system. Estimated wait-time calculations were made in the backend server code and sent to the frontend using the get-wait-time endpoint. We used the Material UI library and Tailwind CSS for the user interface. In-app messaging features were managed through the Stream Chat API.

The main challenge we ran into was implementing the in-app notification system that requires websocket communication between the client and server and setting up the server on Azure such that it allows different computers to interact with the app seamlessly. Initially we also planned to allow users to view all available chats including the ones they were not originally invited to, but the Stream Chat API role permission restrictions prevent us from enabling that functionality.

The instructions for setting up the codebase is included in the README.md in the [project directory](https://www.google.com/url?q=https://github.com/UWSocialComputing/power-hour-code&sa=D&source=editors&ust=1685779044617837&usg=AOvVaw0OgG4CNYT4T-noK86p1Cl9). For future work, we could implement the tool from the TA’s perspective to interact with students in the queue, and incorporate a kudos system for students to send appreciation notes to each other and their TAs.