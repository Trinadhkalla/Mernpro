This is a full-stack MERN (MongoDB, Express, React, Node.js) web application for a blog platform. It allows users to create accounts, add blog posts, edit them, delete them, and view posts from other users. Admins have additional privileges to manage user roles and approve or give feedback on posts.
npm(Node Package Manager)
For doing mern project we should have MongoDB server, node.js application and visual Studio code

Installation:
for Backend Service
Initailze Node and Express Server
npm init
npm i express nodemon cors mongoose bcrypt jwt

for Frontend 
npm init 
npm i create-react-app filename
npm i axios(To render API's)
Import state hooks(use state,use effect)
And we can import what requirements we want

For Starting the server
 npm start

Features:
User Authentication: Registration and login for users.
User Roles: The ability for an admin to update a user's role between 'admin' or 'user'.
Post Management: Users can create, edit, delete, and view their posts. Posts can be viewed by other users.
Admin Panel: Admins have access to approve or reject posts, give remarks, and manage user roles.
Comments: Users can comment on posts, and the comments will display with the username and timestamp.
Post Authorization: Admins can authorize or request corrections on posts before they go public.

Api Endpoints:
route.post("/adduser",adduser)
route.post("/login",login)
route.post("/addpost",islogin,addpost)
route.get("/get",getposts)
route.get("/getbycat/:cat",getbycat)
route.get("/getdonebyme/:uid",islogin,getdonebyme)
route.delete("/delpost/:pid",islogin,delpost)
route.put("/upd",islogin,upd)
route.get("/getrposts",islogin,getrposts)
route.get("/accept/:pid",islogin,accept)
route.put("/updrv",islogin,updrv)

Acknowledgements
MongoDB
Express.js
React
Node.js


