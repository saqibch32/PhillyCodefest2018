# PhillyCodefest2018
### TuTum: Secure the Future
###### *Created by [Mouaz Alhindi](https://github.com/MouazAlhindi), [Shane Staret](https://github.com/SStaret43), [Leander Jeyasingh](https://github.com/Leajey), and [Carlos Chavez](https://github.com/almightmustang1998) as part of the 2018 Philly Codefest hosted at Drexel.*
A school security system that prevents internal and external threats called *TuTum - Secure the Future*. This would  be an application that administrators, security guards, and teachers could use to protect students from other students and external sources.
________________________________________________________________________________________________________________________________

**The primary users of this application are teachers, administrators, and security guards**. It is important to note that students will not have access to this application by any means, as there is great potential that it would be abused.
________________________________________________________________________________________________________________________________

**To prevent external threats**, devices can be put around the school campus entry points to detect movement at unusual times, prompting an alert to be sent to all security guards. Their is a tiered threat level system, so if a guard goes to investigate an alert (whose threat level is defaulted to 0) and finds that it is just an animal, then they can put the alert to the lowest threat level (-1) which resolves the alert. But, if it turns out its a person with a gun, then they can bring it to the highest threat level (2), indicating an emergency which immediately alerts all other security guards, administrators, and teachers. This also immediately alerts the police force as well.
________________________________________________________________________________________________________________________________

**To prevent internal threats**, the attendance system would be heavily involved. We would keep track of where the student was for the previous period and where they should be currently. So, if a student was marked present in their previous class, but is now marked absent for their current class, an alert would be sent to all security guards indicating a student is in the building but not where they are supposed to be. The default threat level for this "student alert" is 0, meaning there is a potential threat. However, teachers and administrators have the ability to flag a student as being potentially dangerous. This would be done because of past behavior. If a student alert is sent out for a student who has been flagged, then the threat level would change from 0 to 1, meaning the security guards should give a higher priority to finding what this student is doing in the building but away from class.
________________________________________________________________________________________________________________________________

**There are two kinds of alerts**, which have been mentioned previously: student and security alerts. A security alert consists of a level, a message, and a room number if a teacher is creating an alert, or a sector (location on campus) if a security guard is creating an alert (optional). All users of this application can create security alerts, however, only the attendance system taken by teachers can signal a student alert. A student alert consists of a level and a message. As stated above, student alerts are when students were previously in the building, but for some reason are not in their current class, whereas security alerts are all other security threats. For example, if a student pulls out a weapon in class, a teacher can immediately pull out their app and signal a security alert to be sent at level 2 (emergency).
________________________________________________________________________________________________________________________________

**There are four different levels of threats**, whose numerical values range from -1 to 2. A threat with a level of -1 indicates an alert that has been **resolved**. The alert was at a different level beforehand, but the threat was successfully stopped or there was no actual threat, so a security guard changed the level to -1. A threat level of 0 indicates that there may be a **potential** threat. Security alerts created automatically by devices along campus are set to send an alert with a default threat level of 0. Student alerts for a non-flagged student are also defaulted to a threat level of 0. A security guard can then investigate the threat and determine whether it should be changed to a different level. A threat level of 1 indicates that a threat **needs to be investigated further**. This is the default threat level for a student alert on a student that is flagged, meaning that security needs to not just find the student, but also investigate what they were doing while they were not in their class and where they were. A security guard may also assign this level if more information about an alert is needed. A threat level of 2 indicates an **emergency**. Anything that can/will put someone within immediate harm will be cast as a level 2 alert. A student pulling out a weapon, an unknown person trying to break into an entrance, a bomb threat, etc. would all be considered emergencies with a threat level of 2. If an emergency is indicated, the local authorities are immediately notified, as well as all administrators, teachers, and security guards.

________________________________________________________________________________________________________________________________

**The UI we designed for this system still needs much work**. The idea was that we would have a login screen, where teachers, administrators, or security guards could login. Depending on what kind of staff they were, the UI would look different. For example, teachers could take attendance through the app, but security guards couldn't. However, security guards could resolve alerts and change alert levels, while teachers couldn't. The administrators would be like teachers, however, they wouldn't have the ability to take attendance. We also wanted to create a statistics frame that could be viewed by anyone. This would hold basic information, like # of security guards, students, and teachers, and different sector locations, etc. During the codefest, we only managed to complete the login system, and we created the backbone of the security guard and teacher interfaces. However, they are not fully functional.
________________________________________________________________________________________________________________________________

Overall, this project was a great idea and the frontend and backend were both completed, however, the UI still needs much work. This system could also be implemented within an office or any other building that has many people within it and a need for extra security. I plan on personally continuing with this project, possibly with the other contributors (Mouaz Alhindi, Leander Jeyasingh, and Carlos Chavez) as well.
