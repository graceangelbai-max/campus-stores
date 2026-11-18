# Campus Stores

Campus Stores is a Product Engineer work sample set at a fictional campus media equipment desk. Work through a club’s screening, from equipment pickup to a partial return and the next morning’s handover. Open **Candidate brief** in the app for the assignment.

## Candidate submission: Handover snapshot

### What I kept

The **Loan register** treats every physical unit as its own slip. At Friday’s Film Society pickup, it only permits an approved equipment type and prevents the same type from being issued twice against the same request. That is a useful guardrail at a busy counter: the person issuing the kit can stay quick without accidentally substituting or over-issuing equipment.

### What I changed

The difficult moment is the Friday 7:30 pm partial return. Kabir returns the projector and speaker, while Leela keeps the adapter until the morning. The original experience leaves the next shift to reconstruct that state from a mix of loan slips and desk-book messages.

I added a **Handover snapshot** at the top of the **Desk book**. It is a small next-shift view generated from the open loan slips. For every outstanding unit it shows:

- the physical asset ID and equipment type;
- its slip number, request club, collector, and due time;
- a Film Society count during the screening scenario; and
- context-specific guidance as the sample shift moves from pickup to partial return to the Saturday handover.

The snapshot updates automatically when a return is recorded, so the desk book remains a handover tool rather than a second manual checklist.

### Walkthrough

1. At Friday pickup, issue the Film Society projector, speaker, and USB-C to HDMI adapter as individual loan slips.
2. Move the story to the return time, then record the projector and speaker returns in the Loan register.
3. Open the Desk book. The Handover snapshot keeps the adapter visible with its exact unit, slip, club, collector, and due time.
4. Move to Saturday morning. When Leela returns the adapter, match it to the remaining Film Society slip and record the return. The snapshot changes immediately.

### What I would measure at a real counter

I would compare the time from shift start to identifying the correct outstanding unit before and after this change. I would also track how often staff ask a colleague to clarify a partial return. A shorter lookup time and fewer clarification requests would show that the snapshot is helping.

## Run the app

Open **index.html** in a modern browser. The app includes its scripts, styles, and icons and can run offline.

Each browser stores its own sample shift locally when browser storage is available. **Restart sample shift** restores the fictional starting records.

## Source

- **index.html** contains the desk layout, candidate brief, and bundled icons.
- **app.js** contains the sample records, the handover snapshot, and interactions.
- **styles.css** defines the desktop and mobile layouts.

Icon license notices are in [third-party/lucide-LICENSE.txt](third-party/lucide-LICENSE.txt).
