# LoyalCredit
**Built on Trust. Proven by Repayment.**
- HTML Mirror:  [https://roxanneardary.com/loyalcredit-specification/](https://roxanneardary.com/loyalcredit-specification/)  

---

LoyalCredit is an open source, relationship-based credit specification for building, evaluating, and managing credit relationships with individuals and businesses. It provides a progressive lending framework that begins with secured credit and can advance qualified borrowers toward unsecured personal or business loans through demonstrated repayment performance.

LoyalCredit is designed around a simple principle: **credit access is earned through reliable repayment**. Borrowers establish a relationship with a lender through secured lending, build a verifiable repayment history, receive a credit grade based on performance, and can progress through the **Credit Trust Ladder** as their demonstrated reliability increases.

The specification is designed for lenders, financial platforms, businesses, cooperatives, community lending organizations, internal credit systems, and other organizations that want to establish their own relationship-based lending programs without depending on a centralized credit scoring provider.

## Core Principles

- Credit is earned through demonstrated repayment behavior.
- Trust increases through successful payment performance.
- Late payments reduce credit standing.
- Consistent repayment can increase borrowing access.
- Secured lending provides the initial path for establishing a credit relationship.
- An A grade is required for eligibility to progress into unsecured lending.
- Default permanently eliminates the borrower from the lending programs of the specific business that recorded the default.
- A default does not prevent the borrower from seeking financing from another lender.
- Credit decisions should be deterministic, explainable, and auditable.
- Individuals and businesses can participate under the same fundamental credit trust model.
- Repeat successful borrowing strengthens the lending relationship.
- The system should reward reliable borrowers with progressively greater access to capital.
- Credit history belongs to the lending relationship and should not be represented as an unquestionable universal measure of a person's worth or financial character.

---

## Core Modules

### Borrower Profile Module

The Borrower Profile Module establishes the identity and lending profile of each individual or business participating in a LoyalCredit system.

Features include:

- Individual borrower profiles
- Business borrower profiles
- Borrower identification
- Business identification
- Lending relationship identifiers
- Account status
- Credit program enrollment
- Borrowing history
- Relationship status
- Eligibility status
- Association of multiple credit accounts with a borrower
- Separation of borrower identity from individual loan records
- Support for lender-specific borrower relationships

### Credit Account Module

The Credit Account Module manages individual credit relationships between a lender and borrower.

Features include:

- Credit account creation
- Secured credit accounts
- Unsecured credit accounts
- Loan amount
- Outstanding principal
- Interest and applicable charges
- Payment schedule
- Payment due dates
- Account balances
- Account status
- Account opening and closing dates
- Loan term
- Repayment history
- Account-level credit performance
- Current and historical credit grades

### Secured Credit Module

The Secured Credit Module provides the initial lending mechanism through which borrowers establish their LoyalCredit relationship.

Features include:

- Secured loan creation
- Collateral registration
- Collateral valuation
- Collateral-to-loan relationships
- Initial borrowing limits
- Secured borrowing requirements
- Payment schedules
- Principal repayment
- Interest repayment
- Successful loan completion
- Repeat secured lending
- Increased secured borrowing capacity based on demonstrated performance
- Eligibility evaluation for progression through the Credit Trust Ladder

Secured credit serves as the foundational stage of the LoyalCredit system. A borrower can establish trust without initially qualifying for unsecured credit.

### Credit Trust Ladder Module

The Credit Trust Ladder is the central progression system of LoyalCredit.

It measures demonstrated repayment performance and determines how a borrower progresses through increasingly trusted lending relationships.

The ladder can include progressive levels such as:

- Initial secured borrower
- Established secured borrower
- Trusted borrower
- A-grade borrower
- Unsecured borrower
- Preferred borrower

Features include:

- Credit progression levels
- Grade thresholds
- Minimum repayment history requirements
- Successful loan completion requirements
- Borrowing capacity progression
- Secured-to-unsecured progression
- Relationship longevity
- Repeat borrowing evaluation
- Trust accumulation
- Trust reduction
- Eligibility gates
- Advancement rules
- Lending restrictions
- Lender-defined progression policies

The Credit Trust Ladder must maintain a clear distinction between **credit performance** and **credit eligibility**. A numerical score may represent performance, while the ladder determines what lending products the borrower is eligible to access.

### Credit Scoring Module

The Credit Scoring Module calculates a borrower score from documented lending behavior.

Features include:

- Starting score
- Positive repayment points
- Late payment deductions
- Payment consistency measurement
- Completed loan evaluation
- Repeat borrowing evaluation
- Loan performance weighting
- Outstanding obligation evaluation
- Score history
- Score changes
- Score explanations
- Deterministic scoring rules
- Lender-configurable scoring parameters

Every score change should be traceable to an identifiable lending event.

The scoring system should never silently change a borrower's score. Each positive or negative adjustment should have a documented reason and timestamp.

### Credit Grade Module

The Credit Grade Module converts credit performance into an understandable lending grade.

A default implementation may use:

- **A:** Excellent credit performance and eligible for secured and unsecured lending
- **B:** Strong credit performance with continued progression toward greater lending access
- **C:** Developing credit performance with secured lending eligibility
- **D:** Elevated lending risk with restricted borrowing access
- **F:** Default or qualifying severe credit failure

The A grade is the primary gateway to unsecured lending.

Features include:

- Grade calculation
- Grade thresholds
- Grade history
- Grade transition rules
- A-grade eligibility requirements
- Grade-based borrowing permissions
- Grade-based lending limits
- Grade explanations
- Lender-defined grade policies

### Payment Performance Module

The Payment Performance Module records and evaluates borrower payment behavior.

Features include:

- Scheduled payment recording
- Payment received dates
- Payment amounts
- On-time payments
- Early payments
- Partial payments
- Late payments
- Payment completion
- Missed payments
- Payment delinquency periods
- Payment status history
- Payment performance calculations

Payment performance is the primary behavioral input into the LoyalCredit scoring and trust progression system.

### Late Payment Module

The Late Payment Module applies defined deductions when borrowers fail to make payments according to the agreed schedule.

Features include:

- Late payment detection
- Days-late calculation
- Configurable late-payment thresholds
- Point deductions
- Grade impact
- Lending eligibility impact
- Borrowing expansion suspension
- Late-payment history
- Transparent penalty calculations

Late payments should reduce trust proportionally according to the severity and duration of the delinquency.

### Default and Elimination Module

The Default and Elimination Module defines the terminal state of a lending relationship.

A qualifying default permanently eliminates the borrower from all lending programs operated by the specific business that recorded the default.

Features include:

- Default detection
- Default qualification rules
- Default event recording
- Immediate lending suspension
- Permanent lender-specific elimination
- Elimination from secured lending
- Elimination from unsecured lending
- Elimination from loan renewal programs
- Elimination from Credit Trust Ladder progression
- Elimination from future borrowing programs operated by that lender
- Immutable default history
- Audit records

LoyalCredit does not define a rehabilitation or reinstatement process following default.

The borrower may seek financing from another lender. LoyalCredit's elimination rule applies to the specific lending business and its lending programs that recorded the default.

### Unsecured Credit Module

The Unsecured Credit Module manages lending that does not require collateral and is available only to borrowers who satisfy the applicable progression requirements.

Features include:

- A-grade eligibility verification
- Unsecured loan applications
- Unsecured borrowing limits
- Loan approval rules
- Payment schedules
- Unsecured loan performance tracking
- Repeat unsecured borrowing
- Unsecured borrowing capacity increases
- Continued grade monitoring
- Automatic eligibility suspension following qualifying performance deterioration
- Default detection

Unsecured lending represents earned access to greater trust and should not be treated as an automatic entitlement based solely on a numerical score.

### Borrowing Capacity Module

The Borrowing Capacity Module determines how much capital a borrower can access at each stage of the Credit Trust Ladder.

Features include:

- Initial borrowing limits
- Secured borrowing limits
- Unsecured borrowing limits
- Grade-based limits
- Repayment-history-based limits
- Outstanding balance calculations
- Exposure calculations
- Aggregate borrower exposure
- Repeat-loan capacity
- Capacity increases
- Capacity restrictions
- Lender-defined maximum exposure

Borrowing capacity should be determined independently from the underlying credit score so lenders can establish transparent lending policies.

### Loan Renewal Module

The Loan Renewal Module manages repeat borrowing and renewal opportunities for borrowers who remain eligible.

Features include:

- Loan renewal evaluation
- Previous loan performance analysis
- Renewal eligibility
- Renewal limits
- Renewal terms
- Repeat borrowing
- Credit Trust Ladder progression
- Updated borrowing capacity
- Renewal denial following qualifying negative performance
- Relationship-based lending incentives

Successful repayment should create opportunities for continued borrowing and stronger lending relationships.

### Relationship Management Module

The Relationship Management Module treats credit as an ongoing relationship rather than a series of isolated transactions.

Features include:

- Borrower relationship history
- Repeat borrowing history
- Successful loan history
- Relationship duration
- Trust progression
- Preferred borrower status
- Repeat-business incentives
- Borrowing opportunities based on historical performance
- Relationship-level eligibility
- Lender-defined relationship policies

The objective is to create a sustainable lending relationship in which reliable borrowers receive progressively greater opportunities.

### Credit Decision Module

The Credit Decision Module combines borrower status, score, grade, ladder position, loan history, payment behavior, and lending policies into an auditable lending decision.

Features include:

- Secured loan eligibility
- Unsecured loan eligibility
- Renewal eligibility
- Borrowing capacity determination
- Grade verification
- Default verification
- Eligibility rules
- Lending policy evaluation
- Approval decisions
- Denial decisions
- Decision explanations
- Decision audit trails

Every decision should identify the rules and borrower information that produced the result.

### Audit and Provenance Module

The Audit and Provenance Module records how credit decisions and score changes were produced.

Features include:

- Credit event history
- Score change history
- Grade change history
- Lending decisions
- Payment records
- Default events
- Eligibility changes
- Rule versions
- Timestamps
- Account identifiers
- Decision provenance
- Immutable audit records
- Historical reconstruction

The audit system should make it possible to reconstruct the borrower's credit standing at any point in the lending relationship.

### Policy Engine Module

The Policy Engine allows each lending business to define its own lending policies while maintaining the LoyalCredit framework.

Features include:

- Score thresholds
- Grade thresholds
- Payment rules
- Late-payment rules
- Default rules
- Borrowing limits
- Secured lending requirements
- Unsecured lending requirements
- Credit Trust Ladder progression rules
- Renewal policies
- Exposure limits
- Business-specific lending policies
- Policy versioning

The policy engine should separate the underlying specification from lender-specific risk policies.

### Privacy and Data Governance Module

The Privacy and Data Governance Module governs the collection, storage, access, retention, and disclosure of borrower information.

Features include:

- Data minimization
- Borrower data access controls
- Lender access controls
- Credit record permissions
- Data retention policies
- Audit logging
- Sensitive financial information protection
- Account-level data isolation
- Data export
- Data deletion policies where legally permissible
- Disclosure controls
- Privacy-preserving identifiers

LoyalCredit implementations should comply with applicable financial, privacy, consumer protection, lending, and data protection requirements in the jurisdictions where they operate.

## Optional Plugin Modules

Optional plugins extend LoyalCredit without changing the core specification.

### External Credit Reporting Plugin

Provides optional integration with external credit reporting systems.

Features may include:

- Credit bureau reporting
- Credit bureau data retrieval
- External credit history comparison
- Reporting compliance workflows
- Dispute management
- External credit record reconciliation

External reporting must remain separate from the internal LoyalCredit score.

### Banking Integration Plugin

Connects LoyalCredit to banking and financial account systems.

Features may include:

- Account verification
- Payment verification
- Balance verification
- Transaction synchronization
- Automated payment detection
- Bank account linking

### Payment Processing Plugin

Provides payment processing integrations.

Features may include:

- Electronic payments
- Automated payments
- Payment confirmations
- Payment reconciliation
- Failed payment notifications
- Payment processor integration

### Identity Verification Plugin

Provides optional borrower identity verification.

Features may include:

- Individual identity verification
- Business identity verification
- Document verification
- Identity matching
- Verification status
- Fraud detection integrations

### Business Verification Plugin

Provides additional verification capabilities for business borrowers.

Features may include:

- Business registration verification
- Business ownership verification
- Business status verification
- Organizational identity
- Business authorization records

### Collateral Valuation Plugin

Provides optional external collateral valuation services.

Features may include:

- Asset valuation
- Property valuation
- Vehicle valuation
- Equipment valuation
- Collateral monitoring
- Valuation history

### Accounting Integration Plugin

Connects LoyalCredit to accounting and financial management systems.

Features may include:

- Loan accounting
- Receivables synchronization
- Payment reconciliation
- Interest calculations
- Financial reporting
- Account balance synchronization

### Risk Analytics Plugin

Provides optional analytical capabilities without replacing the deterministic LoyalCredit scoring system.

Features may include:

- Portfolio analytics
- Lending trend analysis
- Default-rate analysis
- Borrower segmentation
- Exposure analysis
- Performance forecasting
- Portfolio monitoring

Analytical models should not silently modify core LoyalCredit scores or eligibility decisions.

### Notification Plugin

Provides borrower and lender notifications.

Features may include:

- Payment reminders
- Payment confirmations
- Late-payment notifications
- Grade changes
- Credit Trust Ladder advancement notifications
- Renewal notifications
- Eligibility notifications
- Default notifications

### Reporting Plugin

Provides reporting and visualization capabilities.

Features may include:

- Borrower reports
- Loan performance reports
- Credit grade reports
- Trust Ladder reports
- Portfolio reports
- Repayment reports
- Default reports
- Lending performance dashboards

### API Integration Plugin

Provides standardized integration interfaces for external applications.

Features may include:

- Borrower APIs
- Loan APIs
- Payment APIs
- Credit score APIs
- Grade APIs
- Trust Ladder APIs
- Eligibility APIs
- Audit APIs
- Event notifications

## Credit Progression Model

The default LoyalCredit progression model begins with secured lending.

A borrower establishes a lending relationship through a secured loan.

Successful repayment establishes a verifiable performance history.

The borrower's score and grade are updated according to documented repayment behavior.

The borrower progresses through the Credit Trust Ladder as eligibility requirements are satisfied.

An A grade establishes eligibility to apply for unsecured lending, subject to applicable lending policies and capacity limits.

Continued successful repayment can increase borrowing capacity and strengthen the relationship.

A qualifying default terminates the borrower's lending relationship with the specific business and permanently removes the borrower from that business's lending programs.

## Credit Trust Philosophy

LoyalCredit is based on the principle that access to capital should expand in response to demonstrated responsibility.

The system therefore creates a progression:

**Capital Provided → Repayment Demonstrated → Trust Increased → Credit Access Expanded**

Negative behavior produces the opposite progression:

**Late Payment → Trust Reduced → Credit Access Restricted**

A qualifying default produces:

**Default → Lending Relationship Terminated**

This creates a clear and predictable relationship between borrower behavior and future lending access.

## Individuals and Businesses

LoyalCredit supports both individual and business borrowers.

The same fundamental model can be applied to:

- Personal secured loans
- Personal unsecured loans
- Business secured loans
- Business working-capital loans
- Business unsecured loans
- Equipment financing
- Internal employee lending programs
- Cooperative lending
- Community lending
- Private lending programs
- Repeat customer credit programs

Business-specific policies can be implemented through the Policy Engine without changing the core Credit Trust Ladder.

## Deterministic Decision Requirements

LoyalCredit implementations should produce decisions that can be explained to borrowers and lenders.

A decision should be capable of identifying:

- Current credit score
- Current grade
- Current Credit Trust Ladder position
- Payment history
- Late payments
- Outstanding obligations
- Previous successful loans
- Current borrowing capacity
- Eligibility requirements
- Applicable lender policies
- Reason for approval
- Reason for denial
- Reason for restriction
- Default status where applicable

Opaque scoring should not be required for core LoyalCredit functionality.  

## Legal and Regulatory Considerations

LoyalCredit is a technical and financial infrastructure specification. It does not itself constitute legal, financial, lending, underwriting, or regulatory advice.

Implementers are responsible for determining and complying with applicable requirements concerning:

- Consumer lending
- Business lending
- Credit discrimination
- Fair lending
- Consumer protection
- Credit reporting
- Privacy
- Data protection
- Interest rates
- Usury
- Debt collection
- Licensing
- Record retention
- Financial regulation

The internal LoyalCredit score should not automatically be treated as a consumer credit report or external credit score.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/loyalcredit/](https://roxanneardary.com/loyalcredit/)  

---

## License & Notice Requirements

LoyalCredit is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- LoyalCredit specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

**Open Arsenal Hub**  
[https://gitlab.com/Roxanne_Ardary/open-arsenal-specs](https://gitlab.com/Roxanne_Ardary/open-arsenal-specs)
