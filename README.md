Structure :
visitor-management/                     ← Main project folder
│
├── app.py                              ← Main Flask app starter
├── config.py                           ← Config (MySQL, secret key)
├── models.py                           ← User model for login session
├── requirements.txt                    ← Python dependencies
│
├── static/                             ← Static files (CSS/JS/images)
│   ├── css/
│   │   └── style.css                   ← Global styling + gradient headings
│   ├── js/
│   │   └── main.js                     ← JS for tables, modals, export, etc.
│   └── images/                         ← Visitor uploaded images (if needed)
│
├── templates/                          ← HTML templates
1.	│   ├── base.html                       ← Base layout (header, nav, css load)
2.	│   ├── login.html                      ← Admin/Sub-user login page
3.	│   ├── dashboard.html                  ← Main dashboard (visitor list + cards)
4.	│   ├── add_visitor.html                ← Form to register new visitor
5.	│   ├── edit_visitor.html               ← Edit existing visitor info
6.	│   ├── manage_departments.html        ← Add/edit/delete departments
7.	│   ├── manage_hosts.html              ← Add/edit/delete hosts
8.	│   ├── view_visitor.html              ← View single visitor profile (optional)
9.	│   └── export.html                     ← Export data filter page
│
├── auth/
│   └── routes.py                       ← Login, logout logic
│
├── visitors/
│   └── routes.py                       ← Dashboard, add/edit/delete visitor
│
├── users/
│   └── routes.py                       ← Admin creates/deletes sub-users
│
└── schema.sql                          ← MySQL database creation script
└── extensions.py



2. Install requirements.txt
3. Change secret key and password for mysql DB in config.py file.
4. Create the sceama provide in sceama.sql (Note: DB name must be 'visitors').
5. Now run app.py in terminal.
