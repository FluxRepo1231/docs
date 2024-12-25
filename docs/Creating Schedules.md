Schedules in server management are tools that allow you to automate tasks at specific times or intervals. These tasks can include actions like restarting the server, running commands, backing up files, or performing maintenance. By using schedules, you can ensure routine operations happen automatically without manual intervention, improving efficiency and reliability.

1. **Navigate to the Schedules Section**  
   - Find and click on the **Schedules** option in the navigation menu.

2. **Create a New Schedule**  
   - Click the **Create New Schedule** button.
   - Provide the following details:
     - **Schedule Name**: Give the schedule a unique name (e.g., `Daily Restart`).
     - **Cron Expression**: Set the time and frequency using a cron expression. For example:
       - `0 0 * * *` — Runs daily at midnight.
       - `*/5 * * * *` — Runs every 5 minutes.

3. **Add a Task to the Schedule**  
   - Once the schedule is created, click **Add Task**.
   - Choose the type of task to execute:
     - **Command**: Runs a specific command on the server.
     - **Power Action**: Performs actions like restarting or stopping the server.
   - Configure the task:
     - Enter the command or select the power action.
     - Set the task **delay** (e.g., wait 10 seconds before executing).

4. **Save and Enable the Schedule**  
   - Click **Save** to finalize the schedule.
   - Ensure the schedule is **enabled** by toggling the activation switch.

---

## Example Use Cases

### Example 1: Daily Server Restart
1. Create a schedule named `Daily Restart`.
2. Set the cron expression to `0 3 * * *` (runs at 3:00 AM every day).
3. Add a **Power Action** task and select **Restart**.
4. Save and enable the schedule.

### Example 2: Broadcast a Message Every Hour
1. Create a schedule named `Hourly Broadcast`.
2. Set the cron expression to `0 * * * *` (runs every hour).
3. Add a **Command** task with the message:  
   ```plaintext
   say Server maintenance will happen soon.