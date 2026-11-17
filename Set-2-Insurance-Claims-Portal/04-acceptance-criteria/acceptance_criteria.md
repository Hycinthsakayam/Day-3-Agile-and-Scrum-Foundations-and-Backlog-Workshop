# Acceptance criteria

**Question:** Write acceptance criteria in Given / When / Then format for the Claim Registration stories, including a validation failure scenario.

### S1 – Log in with policy number and OTP

_As a policy holder, I want to log in with my policy number and an OTP, so that only I can raise claims on my policy._

**Scenario: Successful login**

```gherkin
Given policy POL-MOT-7781 is active and registered to mobile 98400xxxxx
When I enter the policy number and the correct OTP
Then I see my policy dashboard
```

**Scenario: Validation failure – wrong OTP**

```gherkin
Given I have requested an OTP
When I enter a wrong OTP three times
Then login is blocked for 15 minutes and I see 'Too many attempts'
```

### S2 – Register a motor claim

_As a policy holder, I want to register a motor claim with incident date, place and description, so that my claim is started without visiting a branch._

**Scenario: Claim registered**

```gherkin
Given I am logged in with an active motor policy
When I enter incident date 10-Nov-2026, place and description and submit
Then a claim number like CLM-2026-000123 is shown and sent by SMS
```

**Scenario: Validation failure – future date**

```gherkin
Given I am registering a motor claim
When I enter an incident date after today
Then I see 'Incident date cannot be in the future' and the claim is not submitted
```

**Scenario: Validation failure – policy lapsed**

```gherkin
Given my policy expired before the incident date
When I submit the claim
Then I see 'Policy was not active on the incident date' and the claim is not created
```

### S3 – Register a health claim

_As a policy holder, I want to register a health claim for a hospital stay, so that I can claim reimbursement online._

**Scenario: Claim registered**

```gherkin
Given I have an active health policy
When I enter hospital, admission and discharge dates and submit
Then the claim is created with status 'Registered'
```

**Scenario: Validation failure – dates**

```gherkin
Given I am registering a health claim
When the discharge date is before the admission date
Then I see 'Discharge date must be on or after admission date'
```

### S4 – Save as draft

_As a policy holder, I want to save a half-filled claim as a draft, so that I can finish it later._

**Scenario: Draft saved**

```gherkin
Given I have filled half of the motor claim form
When I tap 'Save draft'
Then the draft appears under 'My drafts' and can be reopened for 30 days
```
