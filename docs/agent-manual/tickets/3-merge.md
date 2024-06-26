# Merging Tickets

Merging becomes necessary when multiple tickets are created for the same issue.

## When should we merge?

Merge tickets when:

1. A customer contacts us multiple times about the same issue.
2. A single issue spans across different communication channels (e.g., phone, WhatsApp, email).

Merging ensures all relevant information is consolidated, providing a complete picture of the customer's concern.

## What Gets Merged?

When tickets are merged:

1. All messages from newer tickets are transferred to the original ticket.
2. Notes and internal comments are also migrated to maintain context.
3. The original ticket becomes the primary record for the issue.


## How Does AIRES Handle Merging?

### Call-type tickets
AIRES employs a proactive approach to minimize the need for merging call-type tickets:

<figure markdown="span">
    ![img](img/image.png){width="75%"}
    <figcaption>Merge flowchart for Call-type tickets</figcaption>
</figure>


1. **Retrieval**: At the start of each conversation, AIRES retrieves all open tickets associated with the customer, irregardless of channels.
2. **Analysis**: AIRES analyzes the conversation content to identify potential duplicate issues.
3. **Updating**: If a duplicate is detected, AIRES confirms with the customer and updates the original ticket with new information.

As an agent, you'll work with tickets that are too complex for AIRES to handle. That means that if its a duplicate issue, AIRES would already have handled it accordingly. 

<figure markdown="span">
    ![img](img/image.png){width="75%"}
    <figcaption>AI Suggestion for duplicate ticket</figcaption>
</figure>

However on edge cases, on the AI suggestions tab, you may receive prompts from AIRES when it detects a potential duplicate. Click on the "Fix now" button to merge the ticket with the AI's proposed original ticket. Modify the "Original Ticket" field if needed.

### WhatsApp and Email-type tickets

These tickets are created automatically when customers contact support. AIRES handles merging for these tickets as follows:

<figure markdown="span">
    ![img](img/image.png){width="75%"}
    <figcaption>Merge flowchart for WhatsApp and Email-type tickets</figcaption>
</figure>

1. **Retrieval**: Same as Call-type tickets.
2. **Analysis**: Same as Call-type tickets.
3. **Merging**: If a duplicate is detected, AIRES confirms with the customer and merges the original ticket with new information.

Similarly, AIRES will prompt you to merge if it detects a duplicate ticket.