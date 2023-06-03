# User Research
## Project Overview
Our project aims to explore the feasibility and potential impact of adding new features to an office hours management tool used in CSE courses. The goal of this study is to assess the effectiveness of existing CSE Office Hour methods and survey how to improve student satisfaction and academic performance. The study will involve gathering feedback from both students and TAs to identify areas for improvement of a tool to maximize office hours productivity.

## Target Audience
The target audience for this office hours management tool includes CSE (Computer Science and Engineering) Teaching Assistants (TAs) and students who want to enhance their learning / teaching experience. The TAs will use the tool to efficiently manage the office hours queue and assist students with their questions. The automatic queue management feature will allow TAs to prioritize student questions based on their severity and length, ensuring that urgent questions are addressed promptly. Meanwhile, the peer-to-peer collaboration feature will encourage students to help each other during office hours, for a more supportive learning environment. Both TAs and students will benefit from the improved efficiency and effectiveness of office hours.

## User Research Method
### User Interviews
We came up with two different sets of interview questions, one for TAs and one for students. Since TAs are also students in CS classes, our TA interviews also covered some aspects of the student questions asking them to answer from the student perspective. These interviews gave us more in-depth insight on how office hours are being run in the intro series, 100-level CS courses, as well as 300-level CS courses.

The three TA interviews involve experienced TAs who have TAed for intro series, various 300-level CSE courses, as well as other 100-level non-intro series that include non-major students. One of the TAs has experience with both theory-heavy courses (CSE 311) and programming-heavy courses (intro series and CSE 331). The two student interviews involve juniors that have experience with many CSE courses. In particular, they shared anecdotes about CSE 311, 312, 331, and 332 office hours.  

### Survey
We designed a survey to collect more quantitative data. The survey starts with student perspective questions, and if the responder self-identifies as a TA in a CSE course at the end of the student section, they will also be presented with the TA-related questions. We distributed the survey in TA staff chats we have access to, the discussion board of the capstone course, and various group chats. We have received 11 responses in the survey with 5 students and 6 TAs. 

## Analysis

### Activity
Our research focuses on the act of providing (from the TA perspective) and receiving (from the student perspective) help in office hours for CSE courses. The majority of students attend office hours with the goal of resolving an issue. Students usually get help with lecture material, written homework questions, and debugging. Some TAs also report students “hanging out” and use office hours to work on their course assignments.

### Environment
Office hours happen in-person and online. In-person is most prominent, where students will go to a designated space on campus and receive help from a TA. During the COVID pandemic, most courses substituted with virtual office hours on Zoom. While courses have returned to majority in-person office hours, virtual is still an option at the discretion of the instructor or TA.

### Interaction
We observed three main forms of interaction during office hours:
1. **Student-TA interaction:** The TA or the office hours tool will usually direct students towards a queue, and the TA will help each student individually in order of the queue. When the queue is very long or when questions are more concept-based, TAs would help a group of students with similar questions.

2. **Student-student interaction:** Students collaborate with each other to resolve their issues. The level of collaboration varies per course due to different policies and type of content (programming-heavy vs theory-heavy). Both students and TAs reported that students are less inclined to collaborate in office hours for programming/debugging since looking at each other’s code could be considered academic misconduct, unless partner work is allowed. Collaboration is generally more productive for written problem-sets that focus more on theory. TAs can encourage collaboration by grouping students with similar questions when the queue is too long. While most students think collaboration is helpful, some mentioned in the survey that individual questions could be crowded out by a group when the majority wants to work on a different question.

3. **TA-TA interaction:** Office hours are hosted by multiple TAs in the same space at the same time. Many TAs preferred the co-TA office hours format, noting that it’s easier to get through the queue together and they can bounce ideas off each other during the session.

### Objects
There are a variety of tools used to manage in-person office hours queues, from specialized software solutions like the old in-house IPL queue and now TheDigitalHand, to custom automated solutions like spreadsheets with macros, to the most basic yet effective method of writing names on a whiteboard. Zoom waiting rooms are also used for online office hours. Students reported negative experiences with that method because they could not track the number of other students in the queue or interact with them if necessary. Whiteboards are useful for TAs to explain concepts by drawing diagrams during in-person office hours. However, the Zoom annotation tool as a substitute for virtual office hours is not as effective since it is hard to draw with a mouse.

### Users
We had two primary user profiles:
1. **TAs:** Students (generally upper-classmen, Masters, or PhD) who have taken the course or have extensive experience in the subject matter. Their goal is to help students understand course topics and answer questions about assignments
2. **Students:** Undergraduate students taking the course. Their goal is to get clarification on the course content and help on assignments.


## Key Takeaways and Design Opportunities
Based on the feedback collected from students and TAs, the following are the key takeaways for the office hours managing tool:
1. **Prioritize general questions:** Students appreciate when TAs take general questions first before moving onto 1:1s. This allows for a more inclusive learning environment and encourages students to participate.
2. **Keep a list of solved bugs:** Maintaining a list of previously solved bugs can be helpful for students who may encounter similar issues in the future.
3. **Encourage peer-to-peer collaboration:** Students want to work with their peers during office hours. Encouraging collaboration and providing tools for peer-to-peer interactions can lead to a more engaging learning environment.
4. **Improve the queuing system:** A queuing system that takes into account the severity and length of student questions, can reduce wait times and ensure that urgent questions are addressed promptly.
5. **Dedicated office hours for peer-to-peer collaborations:** This creates a space for students to work together and learn from each other. Alternatively, having individual-focused office hours can help students with specific questions.
6. **Provide estimated wait-times:** Accurate wait-times allow students to plan ahead and engage in other activities while waiting.
7. **Make use of wait-times:** Students often spend 30 minutes to an hour at office hours but only 10 minutes getting help from the TA. Access to alternative tools and resources while waiting would help them to stay productive.
8. **Limit time with each student:** TAs and students are put in an awkward position when a student takes too long at OH so a system that automatically reminds students to wrap up their question would be helpful.

