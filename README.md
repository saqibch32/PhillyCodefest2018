# PhillyCodefest2018
### TuTum: Secure the Future
A school security system that prevents internal and external threats called "TuTum - Secure the Future". This would  be an application that administrators, security guards, and teachers could use to protect students from other students and external sources.
________________________________________________________________________________________________________________________________

**To prevent external threats**, devices can be put around the school campus entry points to detect movement at unusual times, prompting an alert to be sent to all security guards. Their is a tiered threat level system, so if a guard goes to investigate an alert (whose threat level is defaulted to 0) and finds that it is just an animal, then they can put the alert to the lowest threat level (-1) which resolves the alert. But, if it turns out its a person with a gun, then they can bring it to the highest threat level (2), indicating an emergency which immediately alerts all other security guards, administrators, and teachers. This also immediately alerts the police force as well.

**To prevent internal threats**, the attendance system would be heavily involved. We would keep track of where the student was for the previous period and where they should be currently. So, if a student was marked present in their previous class, but is now marked absent for their current class, an alert would be sent to all security guards indicating a student is in the building but not where they are supposed to be. The default threat level for this "student alert" is 0, meaning there is a potential threat. However, teachers and administrators have the ability to flag a student as being potentially dangerous. This would be done because of past behavior. If a student alert is sent out for a student who has been flagged, then the threat level would change from 0 to 1, meaning the security guards should give a higher priority to finding what this student is doing in the building but away from class.

There are two kinds of alerts, which have been mentioned previously: student and security alerts. All users of this application to create security alerts, however, only the attendance system taken by teachers can signal a student alert. As stated above, student alerts are when students were previously in the building, but for some reason are not in their current class, whereas security alerts are all other security threats. For example, if a student pulls out a weapon in class, a teacher can immediately pull out their app and signal a security alert to be sent at level 2 (emergency).

Overall, this project was a great idea and the frontend and backend were both completed, however, the UI still needs much work. This system could also be implemented within an office or any other building that has many people within it and a need for extra security.
