## Code level

### Stakeholders

* Individual Developer
* Pair Programming Mentor
* DBA
* Security Team

### Failure Points

* Logic flaws
* Security flaws
* Code standards issues

### Guards

* Test Driven Development
* Red/Green/Refactor
* Linting tools
* Testing Docker containers
* Pair programming
* Query analysis
* Static code analysis

## Commit level

### Stakeholders

* Security Team Member for Signoff
* Engineering Team Lead for Signoff

### Failure Points

* Force pushes
* Merge conflicts

### Guards

* Master branch protections
* 3 member signoff before master merge
* Commit hooks

## Test level

### Stakeholders

* Individual Developer
* QA Team

### Failure Points

* Broken tests
* Stale tests
* False positive tests

### Guards

* Weekly failure testing to catch broken tests
* Daily cron runs of test suite against mock prod environment

## Deployment level

### Stakeholders

* SysOps Team
* Individual Developers
* Support Team
* Customers

### Failure Points

* Broken deployments
* Dropped customer traffic

### Guards

* Blue/Green deployment
* Traffic re-routing
* Pre deployment spare instance warmup
* Comms out to support in order to verify proper staffing levels

## Runtime level

### Stakeholders

* Security Team
* SysOps Team
* Engineering Teams
* Customers
* Support Team

### Failure Points

* High resource usage
* Slow queries
* Malicious actors
* Provider downtime

### Guards

* Comms out to support for new feature awareness and appropriate categories for issues regarding the component
* System resource alarms for various metrics and slow DB log alerts
* Instant maintenance page switchover capabilities
* Status page on redundant providers
* Application firewalls
* Database replicas
