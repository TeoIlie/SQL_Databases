# COVID Vaccine DB Website
## Intro
A fully functioning web-based interface for the covid vaccination database, using `ER_diagram_vaccines.drawio`.

## Explanation
**PHP** is used for functionality, **SQL** for database access, and **HTML** for the website itself. Functions include:

- Record a vaccination for a patient.  You should first ask the person for their OHIP number.  If the patient doesn't exist in the database, you will need to prompt for the patient information (don't worry about spouse) and add the patient first before asking for vaccination data. 
  - Once the patient is in the database, ask for the vaccination data: which clinic the vaccine was administered at (list them and let the user choose), the lot number of the vaccine that they were given.
  - Record the vaccination.
  - List all vaccinations for this patient after you update the vaccination table.
- Allow the user to choose a vaccine type and display all the vaccination sites that have (or will) offer that type of vaccine along with the total number of doses that have shipped to that site.
- Allow the user to choose a patient (from the list of patients in the database) and show their vaccination status -- ie. the patient's name, ohip number, the date the vaccine was given and the type of vaccine that was given.
- Show a listing of all workers that work at a vaccination site (chosen by the user) .  Show their name and whether they are a doctor or a nurse.

## Sites Explanation
- `covid.php` is the homepage where you can access subpages through buttons and text input
  - `sites_page` displays site vaccine availability
  - `workers_page` displays doctors, nurses at different sites
  - `status_page` displays the vaccine records of a selected patient
  - `add_patient_page` records patient info to add a new patient record, using `add_patient.php`
  - `add_record_page` records vaccine info to add a new vaccine record, using `add_vaccine_record.php`
