# Lesson Plans
> Lesson plans and instructional assets for all required course sessions
 
---

### Asset Storage

> Subfolder structure within a given `lesson`:

- /`Images` <-- storage for any visual assets needed
- /`Data` <-- storage for any datasets required for lesson activities or instructor demos
- /`Activities` <-- storage for discrete lesson activities
  - //`01-audience_title` <-- should contain instructions and prompts
    - ///`Solved` <-- separate solution code 

> We recommend zipping all activity prompts and starter data/code (minus solutions) into a single zip folder to share with students at the beginning of the lesson. 

#### Activity Folder Naming Conventions

- `/01-Ins_title`: Intended for an instructor to demonstrate function or outputs

- `/02-Stu_title`: Intended for student to practice or complete

- `/03-Evr_title`: Intended for everyone (e.g. a group "code-a-long" led by instructor)

#### Delivery Model

> For graded/credit-bearing courses, we have found that we can increase student participation in lesson activities by removing sample solutions ahead of time. This is doubly important for graded assignment solutions, which should be withheld from students until after submission. Since solutions are stored alongside corresponding assets within our repositories, here are a few options for separating these when delivering the course:

- **IF** sharing lesson materials via Github, create a new repository and paste materials in, minus the solution files. 
    - Example: Clone course repository to local, migrate to `lessons` (or `assignment`) folders, _remove_ the `solved` sub-folders (e.g. cut and paste them over to a new location on your local machine), then "publish" to your new repository. 
    - This should retain all the relevant course content minus the solved materials, which you can then upload/publish/share with students on an as-needed basis (e.g. at the end of each lesson or after assignment submission).

- **IF** sharing lesson files via Google Drive, download materials, separate `solved` content, and upload into Drive
    - Example: Clone course repository to local, migrate to `lessons` (or `assignment`) folders, _remove_ the `solved` sub-folders (e.g. cut and paste them over to a new location on your local machine), then upload resulting folders into Drive (omitting `solved` materials so you can upload and share with students at a later date, on demand).

---

## Copyright
© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
