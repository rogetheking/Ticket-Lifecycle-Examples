# Ticket-Lifecycle-Examples<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


</div>

# 🧠 Technologies Used
- osTicket (Help Desk Ticketing System)
- Microsoft Azure (Cloud Computing)
- Remote Desktop
- Windows 10 Professional x64 22H2

# 📝 Ticket Lifecycle Stages
- Intake
- Assignment & Communication
- Working the Issue
- Resolution

# ♻️ Ticket Lifecycle Examples: From Intake to Resolution

### 📩 Intake
1. Navigate to `localhost/osTicket/index.php` and click the blue `Open a New Ticket` button.

<img src="/images/open-new-ticket.png" alt="Open New Ticket">

2. Proceed to fill out the following fields with the relevant ticket information:
    - **Email Address**: The email address of whoever is submitting the ticket
    - **Full Name**: The full name of whoever is submitting the ticket
    - **Help Topic**: Click on the drop-down menu and select the issue that best fits with the issue in which the ticket is regarding
    - **Issue Summary** In the first field, enter a brief title for the issue and then proceed to the second field where a more detailed description is optional but recommended

In the end-user-created ticket example below, `Jane Doe` (best reached at `jane.doe1999@gmail.com` or `999-999-9999`) is submitting a ticket regarding her trouble to access online mobile banking.

<img src="/images/end-user-ticket.png" alt="End User Ticket">

### 💬 Assignment & Communication
1. Navigate to `localhost/osTicket/scp/login.php` and enter the credentials for the administrator that will assign an Agent to work on the ticket created during Intake.

<img src="/images/admin-credentials.jpg" alt="Admin Credentials">

2. Navigate to `Tickets` > ` Open` and then open the ticket by clicking the ticket number under the **Ticket** column.

<img src="/images/open_ticket_as_admin.png" alt="Open Ticket as Admin">

3. From here, set the **Priority**, **Assign Department**, **Assigned To**, and the **SLA Plan** values for this ticket.

In the example below, the admin first clicks on the greyed out `— Unassigned —` text that's located to the right of **Assigned To**. Then, the admin designates `Luke Skywalker` as the **Assignee**.

<img src="/images/assign-agent-to-ticket.png" alt="Assign Agent to Ticket">

After the agent has been assigned to this particular ticket, the admin sets the **Priority** to `High`, the **Department** to `Support`, and the **SLA Plan** to `SEV-A`.

<img src="/images/filled-ticket-info.png" alt="Filled Ticket Info">

4. Within the ticket tab, you can see the thread of any updates to the ticket and submit updates upon assignment. Once finished, click the orange `Post Reply` button and the ticket gets assigned to the appropriate department and your customer gets notified of this change.

<img src="/images/ticket-timeline.png" alt="Ticket Timeline">

### 🛠️ Working the Issue
1. Navigate to `localhost/osTicket/scp/login.php` and enter the credentials for the Agent that has been assigned to work on the ticket created during Intake.

<img src="/images/agent-credentials.png" alt="Agent Credentials">

2. Once logged in, the Tickets window shows. It will show the ticket number, the last time it was updated, the subject, who submitted the ticket, priority level, and who it is assigned to. The Agent must click on the ticket number to open it so that they can begin working through the problem.

<img src="/images/tickets-window.png" alt="Tickets Window">

3. Once the ticket is opened, you can review all ticket items and the history of the ticket items. This includes who submitted the ticket, who assigned the ticket, and any other ticket activity. The bottom section is where you can leave a reply for the user who submitted the ticket and an internal note to notify management if the ticket has been resolved.

<img src="/images/opened-ticket.png" alt="Opened Ticket">

4. Once the Agent (Luke Skywalker) has reviewed all of the ticket details and identified a solution to the problem, the Agent can then use the **Post Reply** section to write a note to the user (Jane Doe) explaining everything, including the solution, in a professional manner.

<img src="/images/agent-works-the-issue.png" alt="Agent Works the Issue">

### ❤️‍🩹 Resolution

1. Before the user presses the orange `Post Reply` button to send the message to the user, it is important to navigate to the **Ticket Status** drop-down menu and change the value from `Open (current)` to `Closed`.

<img src="/images/close-the-ticket.png" alt="Close the Ticket">

2. Then, osTicket will take the Agent back to the Tickets tab. The Agent will then see a confirmation that the reply was posted successfully. As pictured below, ticket `#325542` by Jane Doe is no longer showing in the **Open** tickets section. Additionally, there is a visual confirmation banner at the top that says `Ticket #325542: Reply posted successfully`.

<img src="/images/ticket-closed-confirmation.png" alt="Ticket Closed Confirmation">

3. To view tickets that have been closed, Agents can navigate to `Tickets` > `Closed` > and then click the appropriate time frame that this ticket is from. From here, the Agent should see closed ticket in question.
