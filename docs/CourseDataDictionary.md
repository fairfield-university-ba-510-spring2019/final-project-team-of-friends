## Data Dictionary _defining every column on every table_

## CATALOGS
| Attribute | Description |
| --- | --- |
| CatID | Surrogate key which identifies a specific course within the catalog. |
| CourseCode | Course's program code plus the number which identifies the specific course. |
| Title | Name of the course. |
| Credits | Number of credits the course counts for. |
| Prereqs | Conditions that need to be met before being eligible for the specified course. |
| Coreqs | Course that must be completed before or taken concurrently with the specified course. |
| Fees | Costs to student associated with the specified course. |
| Attributes | Unique attributes of a specified course. |
| Description | Description of the course content and requirements. |
| CatYear | Year that the catalog was released. |
| PID | Surrogate key which identifies a specific program. |

## COURSES 
| Attribute | Description |
| --- | --- |
| CID | Surrogate key which identifies a specific course. |
| CRN | Course reference number. |
| Term | Season of the year in which the course is offered. |
| Title | The name of the course. |
| Section | Course instance with independent meeting times and students. |
| Cap | Maximum amount of students allowed to enroll in the course. |
| Act | Actual amount of students rolled in the course. |
| Rem | Amount of spots remaining in the course. |
| Credits | Number of credits the course counts for. |
| FID | Surrogate key which identifies a specific instructor.|
| CourseCode | Course's program code plus the number which identifies the specific course. |

## FACULTY 
| Attribute | Description |
| --- | --- |
| FID | Surrogate key which identifies a specific instructor.|
| FName | The professor who teaches the course. |

## PROGRAMS
| Attribute | Description |
| --- | --- |
| PID | Surrogate key which identifies a specific program.|
| Program_Code | Two or three letter code which identifies the program the course is a part of. |
| Program_Name | Full name of the program the course is a part of. |


## COURSE_MEETINGS 
| Attribute | Description |
| --- | --- |
| CMID | Surrogate key which identifies a specific course meeting. |
| Term | Season of the year in which the course is offered. |
| Location | Room number for a given section. |
| Day | One letter code to signify which days of the week a section meets. |
| Start | String of the date and time when a section begins. |
| End | String of the date and time when a section concludes. |
| CRN | Course reference number. |