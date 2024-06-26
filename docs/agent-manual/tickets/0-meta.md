# Ticket Metadata

Tickets in AIRES are used to track customer service requests. All tickets are automatically created as the AI interacts with the system.

<figure markdown="span">
    ![img](img/image.png){width="75%"}
    <figcaption>Ticket Entity in ERD format</figcaption>
</figure>

<figure markdown="span">
    ![img](img/image.png){width="75%"}
    <figcaption>Owner explanation in flowchart</figcaption>
</figure>

Each ticket is visually identified by both an owner logo and a state color.

## Owner

<div align="center" markdown="1">
| Ticket logo | Owner |
|:-----------:|:-----------------:|
| :robot: | AIRES |
| :man_office_worker: | Human agent |
| :red_circle: | Unassigned |
</div>

The owner is the agent assigned to the ticket. AIRES initially handles tickets, but complex cases are marked as unassigned (""). AIRES detects unassigned tickets and notifies the most available agents based on factors like current workload, screen idle time, and time since last request.

## State

<div align="center" markdown="1">
<figcaption style="font-weight:bold">Call-type tickets</figcaption>
| State color | State name | State description |
|:-----------:|:-----------------:|:----|
| :green_circle: | Closed |
| :green_circle: | Merged | All the articles has been migrated to another ticket.
| :yellow_circle: | Open | The ticket is unresolved
| :red_circle: | SLA breached |
</div>

These states help track the progress and urgency of call-type tickets efficiently.

<div align="center" markdown="1">
<figcaption style="font-weight:bold">WhatsApp and Email-type tickets</figcaption>
| State color | State name | State description |
|:-----------:|:-----------------:|:----|
| :green_circle: | Closed |
| :green_circle: | Merged | Same as above
| :yellow_circle: | Open | Whenever the user has answered, and is waiting on ticket owner to reply.
| :yellow_circle: | New | When users hasn't gotten their first response.
| :clock3: | Pending | Whenever the agent has answered, and is waiting on the user's reply. Pauses the SLA.
| :red_circle: | SLA breached |
</div>

These states allow for more detailed tracking of message-based tickets, including response status and SLA considerations.

## Groups

Tickets can be assigned to specific groups, limiting visibility to agents within that group. This optional feature helps manage ticket distribution and reduces clutter.

## Priority

<div align="center" markdown="1">
| Priority | Priority description |
|:-----------:|:-----------------:|
| 3 | High Priority |
| 2 | Normal Priority |
| 1 | Low Priority |
</div>

Priority determines the order in which tickets appear in your interface, ensuring that urgent matters are addressed promptly.