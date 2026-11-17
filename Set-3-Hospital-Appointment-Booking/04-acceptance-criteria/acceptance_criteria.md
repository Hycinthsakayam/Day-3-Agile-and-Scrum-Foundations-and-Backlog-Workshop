# Acceptance criteria

**Question:** Write Given / When / Then acceptance criteria for the booking and cancellation stories (include the 'slot already taken' case).

### S3 – Book a free slot

_As a patient, I want to book a free slot and get a confirmation number, so that my appointment is guaranteed._

**Scenario: Slot booked**

```gherkin
Given Dr. Ramesh Iyer has a free slot at 10:30 on 20-Nov-2026
When I select 10:30 and confirm
Then the slot is booked, I get confirmation number APT-48213 and an SMS
```

**Scenario: Slot already taken**

```gherkin
Given another patient books the 10:30 slot while I am on the confirm screen
When I tap confirm
Then I see 'This slot was just taken' with the next 3 free slots, and no booking is created for me
```

**Scenario: Double booking by the same patient**

```gherkin
Given I already have an appointment at 10:30 on 20-Nov-2026
When I try to book another doctor at 10:30 the same day
Then I see 'You already have an appointment at this time'
```

### S7 – Cancel an appointment

_As a patient, I want to cancel my appointment up to 2 hours before the slot, so that the slot is freed for someone else._

**Scenario: Cancelled in time**

```gherkin
Given my appointment is at 16:00 and it is now 11:00
When I cancel it
Then the status becomes 'Cancelled', the slot shows as free and I get a cancellation SMS
```

**Scenario: Too late to cancel**

```gherkin
Given my appointment is at 16:00 and it is now 14:30
When I try to cancel
Then I see 'Appointments can be cancelled up to 2 hours before' and the booking stays
```

### S6 – Reschedule

_As a patient, I want to reschedule my appointment to another free slot of the same doctor, so that I don't lose my booking when plans change._

**Scenario: Rescheduled**

```gherkin
Given I have a booking at 10:30 and 12:00 is free
When I move it to 12:00
Then 10:30 is freed, 12:00 is booked and the confirmation number stays the same
```

**Scenario: Slot already taken**

```gherkin
Given 12:00 gets booked by someone else while I am rescheduling
When I confirm 12:00
Then I see 'This slot was just taken' and my 10:30 booking is unchanged
```
