<p align="center">
<img src="https://i.imgur.com/haGKChN.png" />
</p>

# osTicket - Ticket Management

This is a continuation of the *osTicket: Configuration Essentials* repository found [here](https://github.com/jgit-arc/osticket-configuration-essentials). The goal of this walkthrough is to become familiar with osTicket as an end-user by creating tickets and resolving them.

---

## Accessing osTicket as an End User

<p>
<img src="https://i.imgur.com/sa6P548.png"/> <br/>
<img src="https://i.imgur.com/urtu8Sz.png"/>
</p>

1. Open the end-user URL (`localhost/osTicket`).
2. Click **Open a New Ticket**.
3. Enter the end-user information (e.g., "Karen") created in the previous walkthrough.
4. Create a mock ticket to simulate working on a real one. The specific information entered isn’t critical for this exercise.
   - Select a **Help Topic** that matches the issue description.
   - Provide a short yet descriptive title in the **Issue Summary** field.
   - Use the larger text field to enter a brief (1-2 sentence) description of the issue.
5. Click **Create Ticket**.

---

## 2. Accessing the Ticket as an Agent and Setting Ticket Properties

<p>
<img src="https://i.imgur.com/pqLf1XN.png" />
</p>

1. Keep the end-user window open! Open a new tab or window and navigate to `localhost/osTicket/scp/login.php`.
2. Sign in using the agent account ("John Doe") created earlier.
   - **Note:** You may be prompted to change your password based on the settings configured previously.
3. Upon logging in, you should see the ticket you just created. If not, click the **Open** or **My Tickets** tabs.
4. Click the name of the ticket. You will see a page similar to the screenshot above.
5. Manually update the ticket properties:
   - Click **SLA Plan** and select the appropriate plan based on the ticket's urgency (e.g., "Sev-A" for immediate issues).
   - Click **Help Topic**, select the most relevant topic, provide a brief justification (e.g., "customer unable to access online banking"), and click **Update**.
   - Note that all changes made to the ticket are logged at the bottom of the page.
6. Click **Assigned To** and assign the ticket to a team or individual (e.g., "Online Banking"). Enter a brief comment and click **Assign**.

---

## 3. Transferring and Completing the Ticket

<p>
<img src="https://i.imgur.com/CXkUH81.png" />
</p>

1. Logout of the "John Doe" agent account and log in as the "Jane" user (or its equivalent).
   - **Note:** The "Jane" account was assigned SysAdmin privileges, so the ticket should still be visible.
2. Open the ticket.
   - If the ticket isn’t already assigned specifically to "Jane," click **Assigned To** and assign it to the account.
3. Use the reply section at the bottom of the ticket to communicate:
   - Regular replies are visible to the customer and are used for asynchronous updates.
   - Use the **Post Internal Note** section for comments visible only to agents with access to the ticket.
4. Click **Status** at the top of the ticket. Set the status to **Resolved/Closed** and click **Close**.
   - Once resolved or closed, the ticket will no longer appear in the agent’s queue.

After closing the ticket, the queue should display **0 tickets**.
