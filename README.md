Low level design


+-------------------------+                     +-------------------------+
|                         |                     |                         |
|      React.js UI        |                     |       Node.js &         |
|-------------------------|                     |    Express.js Backend   |
| - Course List           |<----API Request---->|-------------------------|
| - Course Details        |                     | - /api/users            |
| - User Profile          |                     | - /api/courses          |
| - Instructor Dashboard  |                     | - /api/reviews          |
|                         |                     | - /api/payments         |
+-------------------------+                     | - /api/auth             |
                                                 | - JWT & Middleware     |
                                                 |                         |
                                                 +-----------+-------------+
                                                             |
                                                             | CRUD
                                                             v
                                               +-------------+-------------+
                                               |                           |
                                               |         MongoDB           |
                                               |---------------------------|
                                               | - Users                   |
                                               | - Courses                 |
                                               | - Reviews                 |
                                               | - Payments                |
                                               |                           |
                                               +---------------------------+
                                                 ^            ^             ^
                                                 |            |             |
                +------------------+             |            |             |
                |                  |             |            |             |
                |   Cloudinary     |<------------+            |             |
                |                  |                          |             |
                +------------------+                          |             |
                                                               |             |
                +------------------+                           |             |
                |                  |                           |             |
                |   Nodemailer     |<--------------------------+             |
                |                  |                                         |
                +------------------+                                         |
                                                                              |
                +------------------+                                         |
                |                  |                                         |
                |    Razorpay      |<----------------------------------------+
                |                  |
                +------------------+


# StudyNotion Edtech Project
https://studynotion-frontend-g7ua8jtkl-harshitgoyal12.vercel.app/
