## Data Dictionary _define every column on every table_
</> 
## COURSES Table
| Attribute | Description |
| --- | --- |
| CID | Surrogate key which identifies a specific course. |
| Term | Season of the year in which the course is offered. |
| CRN | Course reference number. |
| Catalog_ID | Abbreviated course identification with course subject and number. |
| Section | Course instance with independent meeting times and students. |
| Credits | Number of credits the course counts for. |
| Title | The name of the course. |
| Meetings | A dictionary of the 'timecodes' data with keys and values. |
| Timecodes | String of course day, meeting times, dates, and meeting location. |
| Primary_Instructor | The professor who teaches the course. |
| Cap | Maximum amount of students allowed to enroll in the course. |
| Act | Actual amount of students rolled in the course. |
| Rem | Amount of spots remaining in the course. |

</>
## FACULTY Table
| Attribute | Description |
| --- | --- |
| FID | Surrogate key which identifies a specific instructor.|
| Primary_Instructor | The professor who teaches the course. |

</>
## COURSE_MEETINGS Table
| Attribute | Description |
| --- | --- |
| CMID | Surrogate key which identifies a specific course meeting. |
| CRN | Course reference number. |
| Term | Season of the year in which the course is offered. |
| Location | Room number for a given section. |
| Day | One letter code to signify which days of the week a section meets. |
| Start | String of the date and time when a section begins. |
| End | String of the date and time when a section concludes. |

</>
## COURSE_CATALOG Table
| Attribute | Description |
| --- | --- |
| CatID | Surrogate key which identifies a specific course within the catalog. |
| Program_Code | Two or three letter code which identifies the program the course is a part of. |
| Program_Name | Full name of the program the course is a part of. |
| Catalog_ID | Course's program code plus the number which identifies the specific course. |
| Course_Title | Name of the course. |
| Credits | Number of credits the course counts for. |
| Prereqs | Conditions that need to be met before being eligible for the specified course. |
| Coreqs | Course that must be completed before or taken concurrently with the specified course. |
| Fees | Costs to student associated with the specified course. |
| Attributes | Unique attributes of a specified course. |
| Description | Description of the course content and requirements. |