## Ruby-Rails-PDF-Generator


## Getting started
Follow the instructions below:


1. Open PDF generator root folder and Open a CLI.
2. Run `bundle install` command to install required gem files
3. Configure Connection with PostgreSQL on `config/database.yml`
4. Set the following to your postgreSQL credentials:

```
  username: postgres
  password: password123
```
5. Run command `rails db:create` to create the database.
6. Run command `rails db:migrate` to migrate the following model/db_tables.
7. Run command `rails db:seed` to insert the faker data on the following article list.
8. Run `npm install` to install latest webpacker.
9. Run `rails server` to start the application.
10. Project will start at `http://localhost:3000`.

`Note:` Only do this if View PDF is showing `Unexecutable wkhtmlpdf` error:

1. Download and install wkhtmlpdf on https://wkhtmltopdf.org/downloads.html
2. Install it on any drive.
3. Open `Ruby-Rails-PDF-Generator\config\initializers/wicked_pdf.rb`
4. Change line number #14 to your wkhtmlpdf installed path:
```js
:exe_path => 'C:\wkhtmltopdf\bin\wkhtmltopdf.exe',
```