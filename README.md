# Secure-Computing
Coursework
**1
XJCOMP3911 Secure Computing
25/26 Coursework
This assignment concerns vulnerabilities in a software application, and how they can be fixed. You should
be able to do the work on any machine that has the Java Development Kit installed.
This assignment is to be done in groups of five or less. You will need to let me know if you cannot
form a group as soon as possible, by sending an email on laha_ale@swjtu.edu.cn
 or let the TA know
via QQ group.
Each member of the group is expected to receive the same mark for the assignment.
This assignment is worth 30% of your overall grade.
Scenario
You are provided with the source code of a Java application in patients.zip. This is a crude attempt by an
inexperienced developer to implement part of a patient records system. The idea is that GPs in a
surgery can login to the application and search for details of patients that they are currently treating.
The application uses Jetty as a built-in web server. Request processing is done by a Java Servlet. Data
storage is provided by an SQLite 3 database, and queries of the database are done using JDBC . HTML
pages are generated using the Freemarker template engine.
Tasks
Task 1: Analysis of Security Flaws

Examine the database used by the application. Amongst other things, this will give you the login
credentials and patient details that you need to test the application.
You can do this on the command line using the sqlite3 tool: the .schema command will tell you
the structure of the database and you can issue SQL queries at the command prompt to examine
its contents. You can exit the tool with .quit.
If you prefer a tool with a GUI, there are many available—e.g., DB Browser .

Compile and run the application from the command line using
./gradlew run
(On Windows, omit the leading ./)

Visit http://localhost:8080
 in a web browser to interact with the application. Use the information
obtained in Step 1 to explore different paths through the application.

Experiment with the web interface to identify any security issues. Make a note of precisely what
the issues are and how you identified them. Collect evidence such as screenshots where
appropriate.

Study the source code of the application if necessary to gain further insight into the application’s
security flaws.

Create a report using a word processor or other documentation preparation tool of your choice.
Give your report the title ‘COMP3911 Coursework’ and include the details of all authors/group
members (name, username and id) on the cover page.
Under a section heading ‘Analysis of Flaws’, write down a list of five flaws you have found. Be
brief here; identify each of the five flaws with a single short sentence.
Then discuss each of the five flaws in more detail. For each flaw, create a suitable subsection
heading, under which you should describe the nature of the flaw and how you discovered it,
providing a suitable example or evidence (e.g., screenshot) in each case.
The entire ‘Analysis of Flaws’ section should be no more than three A4 pages in length, including
figures used as evidence. The contents of this section are worth a total of 10 marks.**

**2
Task 2: Visualisation
Based on the vulnerabilities identified during the security analysis phase, you should provide a
visualisation of these flaws and how they can be exploited.

Develop an attack tree to show how the flaws from Task 1 can be exploited to cause an attacker
to gain access to an asset.

Under a section heading ‘Attack Tree’, explain how the tree has been constructed and how the
flaws can be exploited. You should state any assumption you have made.
This section should be no more than one A4 page in length, including the attack tree. The contents of this
section are worth a total of 5 marks.
Task 3: Implementation of Security Fixes

For each of the flaws identified in the “Analysis of Security Flaws” section, modify the application
(and, if necessary, the database) to fix your chosen flaws.

Test the application to make sure that it still works and that it is no longer vulnerable.

For each fix, explain why it was chosen, based on the attack tree you have developed. This should
be added to a new section in your report, under the heading ‘Fix Identification’. This part should
be no more than one A4 page in length.

Add a new section to your report, with the heading ‘Fixes Implemented’. Write a short (maximum
of two A4 pages) summary of the changes that you have made, explaining in each case how it has
fixed the problem.
Your fix identification, the fixes themselves and the written summary of them are worth a total of 15
marks.
Deliverables
You need to submit (i) your report and (ii) your modified application.
The report should not exceed six A4 pages in length, excluding any cover sheet. The cover sheet must
include the names of all members of the group. It must have the section headings indicated previously.
It must be submitted as a PDF file: do NOT submit a Word document or any other editable document
format. The PDF file must be named report.pdf and it must be put in the same directory as the
build.gradle file.
Note: you will lose marks if you don’t satisfy all of these requirements!
When you have put report.pdf in the correct location, enter the following command:
./gradlew submission
This will create a Zip archive named cwk.zip, containing everything that needs to be submitted.
Deliverables
Submit the file cwk.zip, via the link provided for this purpose in Minerva. Note: The person submitting
needs to also “tag” the other members of the group.
Submission Deadline
The deadline for submission is Wednesday 3rd December 2025 at 23:59.**