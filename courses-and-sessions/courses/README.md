# Courses

A Course is a Curricular object that defines the content and structure of a specific instance of coursework available to the school or program.

There are four main functional areas related to the maintenance and creation of Courses in Ilios. These are detailed below and follow the vertical navigational flow through the page.

## Functional Areas

### Heading 

This area appears at the top of the Course page. It includes everything listed below. 

  - **Back to Courses list:** link back to list of Courses 
  - **Title:** can be edited here - refers to full title (name) of the course, entered on course creation - 200 character maximum
  - **Publication Status:** This is a drop-down menu containing the options for publishing a course - listed below.
    - **Not Published:** initial status at course creation time - can be returned to this later by using **UnPublish**
    - **Publish** or **Publish As-Is:** publishes course 
    - **Review Missing Items:** review desired or required items for course publication
    - **Mark as Scheduled:** sets course to `Scheduled` status
    - **UnPublish:** only available if course has been published - reverts course to `Not Published` status 

### Overview

This refers to the upper area of the screen which is always visible. It provides the main details of the Course including everything listed below.

  - **Course ID:** (external ID) - short title - can be edited here
  - **Clerkship Type:** can be edited / specified here 
  - **Start:** start date for this course 
  - **End:** end date for this course
  - **Level:** course level - can be edited here
  - **Universal Locator:** read-only descriptor field containing database ID

### Details 

This refers to the other course attributes listed below that can be maintained only after "Show Details" has been clicked.

  - **[Leadership](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/course-leadership):** maintain course directors, administrators, and student advisors 
  - **[Objectives](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/course_objectives):** maintain / manage objectives and their relationships to parent (program year) objectives, vocabulary terms, and MeSH terms
  - **[Learning Materials](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/learning_materials):** upload and / or link course learning materials
  - **[Competencies](https://iliosproject.gitbook.io/ilios-user-guide/schools/competencies):** read-only display of competencies that are linked to the associated program year objectives 
  - **[Terms](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/vocabulary_terms):** maintain vocabulary terms associated with this course. These are configured at the [School](https://iliosproject.gitbook.io/ilios-user-guide/schools/vocabularies) level.
  - **[MeSH](https://iliosproject.gitbook.io/ilios-user-guide/additional-information/mesh):** maintain MeSH (Medical Subject Header) terms associated with this course
  - **[Program Cohorts](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/course_actions/edit-course#program-cohorts):** maintain / manage cohort(s) attached to this course

### Session List

  - [**Sessions:**](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/sessions) a full list of all sessions in the course - many edits to sessions can be performed directly from here at the course level (in-line editing).

## Course Attributes

* **Title:** Long title (name) of the course, entered on course creation - 200 character maximum (location: [Heading](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#heading)).
* **Course ID:** Field allowing any internal or external ID up to 255 characters maximum (location: [Overview](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#overview)).
* **Course Year:** Academic year during which instruction will take place. This is set at the creation of the Course. This field cannot be modified using the interface once it is saved.
* **Course Level:** The options for this are set at the [Program](https://iliosproject.gitbook.io/ilios-user-guide/programs#program-attributes) Level. The program duration can be anywhere between 1 and 10. The Course level identifies what point in the curriculum trajectory the course is meant to be addressed by learners, but is not a constraint (location: [Overview](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#overview)).
* **Clerkship Type:** A course may be identified explicitly as a clerkship using this attribute. The available selections are Block clerkship, Integrated clerkship, or Longitudinal clerkship. These may be modified as necessary in the `"course_clerkship_type"` table. The default value for all courses on creation is “not a clerkship” (location: [Overview](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#overview)).
* **Program Cohorts:** Selected from the list of available Cohorts and Programs already entered in the system. Only authorized users from a given program’s home school may edit that program cohort’s relationships to the course (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)). 
* **Start Date:** A calendar selection, which should be within the range of the Course’s academic year (location: [Overview](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#overview)).
* **End Date:** A calendar selection, which should be within the range of the Course’s academic year and must fall after the Start Date (location: [Overview](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#overview)).
* **Competencies**: Competencies listed for a course are a subset of the full set of competency domains for the program(s) associated to the course. When a course Objective is linked into the competency tree via its association to a program Objective, the competency domains to which those program level Objectives are assigned will be displayed and reported as the specific attributes of the course (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)).
* **Objectives:** Free-text entry field. Each Objective entered at the course level may be associated to one or more Program-level Objectives for each program associated with the Course. It is a school-level configurable option to allow Course objectives to be associated with only one Program Year objective, or to allow them to be associated with multiple Program Year objectives. Only authorized users from a given program’s home school may edit the relationships of an Objective to that program’s cohorts. Course Objectives may also be assigned their own MeSH terms and Vocabulary Terms (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)).
* **Leadership:** Populated with a list of previously added members of course leadership. The list is populated with users identified and tagged as having any of these three roles assigned in Ilios: “Director”, "Administrator", or "Stufdent Adviser". All three of these can be reviewed and maintained here (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)).
* **Terms:** Selected from a school-specific, pre-defined list. These are grouped by Vocabularies, which are collections of Terms (school-specific categories of learning) that can be selected and attached (tagged) to many curricular objects within Ilios (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)).
* **MeSH Terms:** Selected by searching the [MeSH](https://iliosproject.gitbook.io/ilios-user-guide/glossary#mesh) database (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)).
* **Learning Materials:** Course level learning materials are available to all Sessions of a Course, and are entered using the Learning Materials search/upload tools (location: [Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses#details)).

## Screen Elements

This shows the Course detail screen (once a Course has been selected and Details have been expanded).

<figure>
  <img src="../../images/course_images/course_top.png" alt="course detail - top">
    <figcaption>
      <p>Course Detail - top part of screen</p>
    </figcaption>
</figure>

## Functionality and Links
### Upper part of screen

1. **Back to Courses List**: takes the user back to the list of Courses
2. **Global Search**: search for anything in Ilios
3. **Language Switcher**: currently can be switched to French, Spanish, or English
4. **Profile Dropdown**: available here -- My Profile, Logout
5. **Help**: link to this guide available anywhere in Ilios
6. **Edit Course Title**: The title can be edited by clicking as shown.
7. **Published Status**: The Course's publication status can be changed here.
8. **Course ID**: The Course ID field can be edited by clicking as shown.
9. **Clerkship Type**: edited here
10. **Start Date**: edited here
11. **Learning Materials Summary**: opens up Learning Materials summary
12. [**Course Summary**](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/course-summary): displays a printable summary overview of the selected course
13. **Rollover Course**: starts the process of rolling this Course over
14. **Course Visualizations**: opens up Visualizations (Graphs) for this Course
15. **End Date**: edited as shown
16. **Level**: edited here
17. **Leadership**: expands to assign Course Directors Administrators, and/or Student Advisors
18. **Objectives**: expands and opens up course objective details and provides access to allow editing of objective text (based on permissions of logged in user)
19. **Search For Learning Material**: to find existing Learning Material
20. **Add Learning Material**: If Learning Material is not found, new ones can be uploaded or attached
21. **Sort Materials**: to change the order in which Learning Materials are displayed to students
22. **Edit Learning Material**: allows for viewing or changing selected Learning Material attributes
23. **Delete Learning Material**: if available, allows for the deletion of Learning Material objects

### Lower part of screen

![course detail - lower](../../images/course_images/course_lower.png)

1. **Competencies**: opens up the read-only listing of Competencies associated with this Course
2. **Terms**: opens up the screen to be used for the maintenance of Vocabulary Terms associated with this Course
3. **Manage MeSH**: allows user to manage MeSH terms associated with this course
4. **Manage Cohorts**: to add or remove Cohorts from the Course
5. **Hide Details**: hides all Course Details with the exception of the [Course Summary Details](https://iliosproject.gitbook.io/ilios-user-guide/courses-and-sessions/courses/edit-course#course-summary-details)

## All Courses (default view)

When first visiting this screen during an Ilios session, the default view is **"All Courses"**, which is shown below. You can limit the number of Courses displayed on the screen by filtering on Course title.

This display can be sorted by the following fields in addition to being filtered by Course title.

### Sort Options

The following columns can be sorted (one at a time) - choose ascending or descending order.

* **Title** - default sort order
* **Level**
* **Start Date**
* **End Date**
* **Status**

To apply any sort order, simply click on the column header to select the sort preference.

The sort order currently applied can be viewed by reviewing the arrow icons and description to the right of the column title. The default sort order is shown below using the 2024 School of Medicine course listing.

<figure>
  <img src="../../images/course_images/default_sort_order.png" alt="default sort order">
    <figcaption>
      <p>Courses List (All Courses)</p>
    </figcaption>
</figure>

**TIP:** It can be helpful to sort by **"Status"** when you want to find out which Courses may not have been published yet. Courses with the status of "Not Published" will appear in the list before "Published" courses based on the A-Z sort order applied here.

<figure>
  <img src="../../images/course_images/course_list.png" alt="course list shown">
    <figcaption>
      <p>Courses List (All Courses)</p>
    </figcaption>
</figure>

## My Courses

By default, all courses for the selected school are displayed. There is a pair of buttons acting as a switch at the top left of the screen which will change into My Courses when clicked as shown below.

**Original appearance:**

![All Courses](../../images/course_images/all_courses_button.png)

**After clicking / toggling:**

![My Courses](../../images/course_images/my_courses_button.png)

The screen is then refreshed to display only the courses with which the logged in user is associated. In this example, the logged-in user is an instructor for one or more session offerings in the three coursed contained in the My Courses list.

The year drop-down menu does apply in this situation. The year selected is 2023 meaning these are the Courses in the selected year associated with the logged-in user.

![My Courses (list of courses)](../../images/course_images/my_courses_list.png)