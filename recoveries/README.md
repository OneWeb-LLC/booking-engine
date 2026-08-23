# Booking Engine Recoveries

Recoveries are named exception paths that return the customer to the strongest valid next step when the Golden Path breaks.

## Recovery families

1. [Activation Recovery](activation.md)
2. [Booking Recovery](booking.md)
3. [Appointment Recovery](appointment.md)
4. [Conversion Recovery](conversion.md)
5. [Payment and Onboarding Recovery](payment-and-onboarding.md)
6. [Reactivation](reactivation.md)

## Recovery contract

Every recovery must define:

- trigger;
- customer state;
- owner or pooled team;
- priority and due time;
- communication and call cadence;
- Call Brief;
- suppression and collision rules;
- success condition;
- exhaustion condition;
- escalation path;
- reporting metrics.

Recoveries describe **why** work exists. Appointments, Live Calls, Assigned Tasks, and Call Queue describe **how and when** users execute it.

