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

6. **Create a View**
   - Set up the view as shown in the file `settings` in this repository.

---

All done!
