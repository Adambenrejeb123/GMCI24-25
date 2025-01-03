# GMCI24-25

## Important Mention

For the login page to be able to access your endpoints, you need to install CouchDB and have a view (endpoint) and document (data) to be fetched correctly.

CouchDB was recommended by the GMCI course in a previous assignment and is needed to demonstrate the SSP feature for Tutors and Students, so please download it.

---

## Steps

1. **Download CouchDB**

   - Visit the website: [Download Apache CouchDB](https://neighbourhood.ie/download-apache-couchdb-win/).

2. **Set Credentials**

   - Use `admin` as the username and password when setting up CouchDB.

3. **Access Fauxton**

   - In your browser, navigate to: [http://127.0.0.1:5984/\_utils](http://127.0.0.1:5984/_utils).

4. **Create a Database**

   - Create a database named `gmci`.

5. **Create a Document**

   - Inside the `gmci` database, create a document with the following content:

   ```json
   {
     "_id": "f4525befa1925f599aabe65e6a000bda",
     "_rev": "2-b682e45a39aa02d9777550dcf8bb11e9",
     "email": "test@test.com",
     "name": "Squidward",
     "lastname": "Tenticles",
     "password": "test",
     "role": "student"
   }
   ```

   -And Another document called "assignments"

   ```json
   {
     "_id": "9e9e2f34fc0e1ead9774ef79ab000f36",
     "_rev": "23-7e769a22f199c381d4a8c27c3d9b0089",
     "entries": [
       {
         "name": "Assignment 1",
         "UUID": "e65dc646-c279-4e53-a3f2-49ff235e679c",
         "student": "Squidward Tenticles",
         "grade": "1.0",
         "expired": true,
         "_attachments": {
           "submission.pdf": {
             "content_type": "application/pdf",
             "data": "BASE64_ENCODED_FILE_DATA"
           }
         }
       },
       {
         "name": "Assignment 2",
         "UUID": "38067ee3-3fbd-47be-942a-e37d58968a53",
         "student": "Squidward Tenticles",
         "grade": "2.7",
         "expired": true,
         "_attachments": {
           "submission.pdf": {
             "content_type": "application/pdf",
             "data": "BASE64_ENCODED_FILE_DATA"
           }
         }
       },
       {
         "name": "Assignment 3",
         "UUID": "38067ee3-3fbd-47be-942a-e37d58968a53",
         "student": "Squidward Tenticles",
         "grade": "N.A",
         "expired": false
       }
     ]
   }
   ```

6. **Create a View**
   - Set up the views as shown in the file `settings` and `settings2` in this repository.

---

All done!
