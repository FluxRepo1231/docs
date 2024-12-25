When you purchase a server, you are provided with **5 databases** that you can create and manage through your server's control panel. Follow the steps below to create a new database:

---

## Steps to Create a Database

1. **Navigate to the Databases Section**  
   - Locate and click on the **Databases** option in the navigation menu.

2. **Create a New Database**  
   - Click on the **Create New Database** button.  
   - You will be prompted to provide:
     - **Database Name**: Enter a unique name for the database (e.g., `my_game_db`).
   - Click **Create** to finalize the database setup.

3. **View Connection Details**  
   - Once the database is created, you will see the following details:
     - **Database Name**: The name you just created.
     - **Connection Info**: The host address or IP used to connect to the database.

---

## Connecting to Your Database

Use the **Database Name** and **Connection Info** to link your application or game server to the database. Typical details include:
- **Host Address**: Found under **Connection Info**.
- **Database Name**: The name you created.

### Example Connection String:
For MySQL:
`mysql -h [Host Address] -u [Database Name] -p`