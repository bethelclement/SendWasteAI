# Initial Data Model

## Primary entities

### Organisation

Estate, SME cluster, hotel, institution, recycler, collector group or public partner.

### User

Role, organisation, contact details, authentication status and consent records.

### Pickup request

Source, material type, estimated quantity, location, requested time, urgency and status.

### Collection event

Collector, timestamps, measured weight, material classification, evidence references, verification status and notes.

### Settlement

Fee, incentive, collector payment, status, reference and approval history.

### Recovery batch

Aggregated verified collection events linked to a recycler or recovery destination.

### Partner report

Reporting period, included verified records, methodology, export status and audit reference.

### Model decision

Model version, input features, score, explanation, reviewer, override status and observed outcome.

## Data separation

- personally identifiable information is stored separately from model features;
- original evidence is stored in object storage and referenced by immutable identifiers;
- derived features can be rebuilt from verified operational records;
- reports distinguish measured, calculated and predicted values.
