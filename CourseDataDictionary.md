## Data Dictionary _define every column on every table_
</> 
## Courses
- term: Season of the year that the course is offered.
- crn: Course reference number
- catalog_id: Abbreviated course identification with course subject and number. 
- section: 
- credits: Number of credits each course counts for.
- title: The name of the course.
- meetings: A dictionary of the 'timecodes' data with keys and values
- timecodes: String of course day, meeting times, dates, and meeting location.
- primary_instructor: The professor signed on to teach the course.
- cap: the maximum amount of students allowed to enroll in the course.
- act: the actual amount of students enrolled in the course.
- rem: the amount of spots available in the course.
</>
## Faculty
- primary_instructor: The professor signed on to teach the course.
- term: Season of the year that the course is offered.
- crn: Course reference number
</>
## CourseMeetings
- crn: Course reference number
- location: Building and room number
- day: One letter code for each day of the week
- start: String of the date and time the course begins.
- end: String of the date and time the course concludes.
</>
## CourseCatalog
- program_code : Identifies the type of program. 
- program_name
- catalog_id
- course_title : Name of the class at the time.
- credits: 
- prereqs: Fundamentl classes needed 
- coreqs
- fees
- attributes
- description