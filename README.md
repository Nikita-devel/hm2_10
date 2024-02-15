# Django Web Project - Quotes Hub

This Django web project replicates the functionality of the website [http://quotes.toscrape.com](http://quotes.toscrape.com) and extends it to include user registration, authentication, author addition, and quote submission features. Additionally, it incorporates database migration from MongoDB to Postgres for improved scalability.

## Features Implemented

### User Authentication and Authorization

- Users can register and log in to the site, allowing personalized interactions.
- Access to specific features, such as adding authors and quotes, is restricted to registered users.

### Author and Quote Management

- Registered users can add new authors to the site.
- Authenticated users can submit new quotes, associating them with existing authors.

### Database Migration

- MongoDB data, including quotes and authors, has been migrated to a Postgres database.
- The migration process is facilitated by a custom script, ensuring data integrity and a smooth transition.

### Public Access

- Non-authenticated users can view author pages and read quotes.
- All quotes are accessible for viewing without requiring user authentication.

### Additional Features

#### Tag-Based Quote Search

- Implemented a tag-based search functionality.
- Users can click on a tag to display a list of quotes associated with that tag.

#### Top Ten Tags

- Created a "Top Ten Tags" block, displaying the most popular tags on the site.

#### Pagination

- Incorporated pagination with "Next" and "Previous" buttons for improved user experience.

#### On-Demand Scraping

- Introduced a feature to scrape data directly from the site upon user request.
- Users can trigger data scraping by clicking a button on the form, populating the site's database.

## Usage

1. Ensure the Django environment is set up.

2. Run migrations to initialize the database:
   ```bash
   python manage.py migrate
   ```

3. Create a superuser account for admin access:
   ```bash
   python manage.py createsuperuser
   ```

4. Start the Django development server:
   ```bash
   python manage.py runserver
   ```

5. Access the admin panel to manage users, authors, and quotes at `http://127.0.0.1:8000/admin/`.

6. Visit the Quotes Hub at `http://127.0.0.1:8000/` to explore the implemented features.

7. Enjoy the features, including user registration, quote submissions, tag-based searches, and more.

## Conclusion

This Django web project successfully replicates and extends the functionality of the original quotes website. It incorporates user authentication, authorization, database migration, and additional features like tag-based search, top tags, and pagination. The inclusion of on-demand scraping enhances the project's versatility, allowing users to update the site's database as needed. The project serves as a robust and user-friendly platform for quotes and author management.
