Prerequisites





XAMPP: Latest version with PHP 8.1 or higher and MySQL (MariaDB)

Installation Steps with XAMPP





Install XAMPP





Download and install XAMPP from https://www.apachefriends.org.



Start the Apache and MySQL modules from the XAMPP Control Panel.



Copy Project to htdocs





Copy the entire ERP system project folder to the XAMPP htdocs directory (e.g., C:\xampp\htdocs on Windows or /opt/lampp/htdocs on Linux).





Example: If the project folder is named erp-system, place it in C:\xampp\htdocs\erp-system.



Import the Database





Open phpMyAdmin by navigating to http://localhost/phpmyadmin in your browser.



Create a new database (e.g., erp_db):





Click "New" in the left sidebar, enter the database name (erp_db), and click "Create".



Select the newly created database in phpMyAdmin.



Click the "Import" tab, then choose the database SQL file (e.g., erp_db.sql) from the project folder.



Click "Go" to import the database.



If the project includes a .env file, update it with the database details (e.g., DB_DATABASE=erp_db, DB_USERNAME=root, DB_PASSWORD=).



Access the Application





Ensure Apache and MySQL are running in the XAMPP Control Panel.



Open your browser and navigate to http://localhost/erp-system/public.



Follow any on-screen setup instructions (if applicable) or log in using default credentials (if provided in the project documentation).

Troubleshooting





Page Not Found: Ensure the project folder is correctly placed in htdocs and the URL includes the /public path (e.g., http://localhost/erp-system/public).



Database Connection Errors: Verify the database name, username, and password in the .env file match the database created in phpMyAdmin. Ensure the SQL file was imported correctly.



SQL Import Errors: Check that the SQL file is compatible with your MySQL/MariaDB version and not corrupted.



XAMPP Not Running: Confirm that Apache and MySQL are started in the XAMPP Control Panel.

Contributing

Contributions are welcome! Please submit a pull request or open an issue on the GitHub repository.

License

This project is licensed under the MIT License. See the LICENSE file for details.
