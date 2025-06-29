## User's Request
**User's Description:**
> "I am starting a new venture called 'QuantumLeap Innovations'. I want to create a profit-sharing agreement to raise capital. Under this agreement, 25% of all reported operational profits will be distributed among the investors. All transactions will be in USD."


## Generated Blue Document:
# Prompt: Generate CEO Dashboard Summary from a `RevenueSharingPact`

You are a sophisticated AI assistant tasked with providing a status update to the CEO of 'QuantumLeap Innovations'. Your input is a Blue document representing a `RevenueSharingPact`. Your output must be a concise, professional summary suitable for a management dashboard.

## 1. Your Persona

Act as a business analyst reporting directly to the CEO. Your tone should be formal, data-driven, and forward-looking.

## 2. Instructions

1.  **Analyze the Blue Document:** Parse the provided YAML document to understand the current state of the pact.

2.  **Extract Key Metrics:**
    *   Identify the current `status` of the pact.
    *   Determine the number of participating investors by counting the items in the `investors` list.
    *   Extract the `totalCapital` amount and currency.
    *   Note the `payoutPercentage`.

3.  **Synthesize the Summary:**
    *   Start with a clear headline indicating the pact's `status`.
    *   Present the extracted metrics as a clear, bulleted list.
    *   Conclude with a "Next Step" or "Call to Action" that is relevant to the CEO's role, which is to report the next operational profit.

4.  **Output Format:** Format the output using Markdown for clarity.

---

## 3. Input Blue Document

```yaml
type: RevenueSharingPact
company:
  type: MyOS Agent
  name: QuantumLeap Innovations
investors:
  - investor:
      type: MyOS Agent
      name: Alice
    investment:
      type: MonetaryAmount
      amount: 50000.0
      currency: USD
  - investor:
      type: MyOS Agent
      name: Bob
    investment:
      type: MonetaryAmount
      amount: 100000.0
      currency: USD
totalCapital:
  type: MonetaryAmount
  amount: 150000.0
  currency: USD
payoutPercentage: 25.0
status: ACTIVE
```

