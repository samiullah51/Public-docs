# Agent Test Questions Guide

This guide provides comprehensive test questions organized by category to test your debt collection AI agent's capabilities.

## ⚠️ Important Note: Intelligent Intent Recognition

**These questions are EXAMPLES only** - they are not hardcoded or statically programmed into the agent. The agent uses **intelligent intent recognition** powered by AI (RAG system with OpenAI) to understand what the caller is asking, regardless of how they phrase their question.

### How the Agent Works:

- ✅ **Understands Intent**: The agent analyzes the caller's question semantically to understand their actual intent, not just matching keywords
- ✅ **Flexible Responses**: Callers can phrase questions in many different ways - the agent will understand them all
- ✅ **Context-Aware**: The agent maintains conversation context and remembers what was discussed
- ✅ **Script Application**: When the agent detects specific objection types (scam concerns, fraud disputes, statute of limitations, etc.), it intelligently applies the appropriate script/rebuttal from its knowledge base
- ✅ **Natural Conversation**: The agent responds naturally and conversationally, adapting to the caller's tone and concerns

### Example:

- If a caller says: _"This feels like a scam call"_ OR _"I don't trust this"_ OR _"This seems fraudulent"_
- The agent recognizes the **scam concern intent** and responds using the appropriate script, regardless of the exact wording

**The questions listed below are just examples** to help you test different scenarios. Feel free to rephrase them, combine them, or ask similar questions - the agent will understand and respond appropriately.

---

## 📋 Table of Contents

1. [Information Verification](#information-verification)
2. [Balance & Debt Questions](#balance--debt-questions)
3. [Payment Questions](#payment-questions)
4. [Case Information](#case-information)
5. [Payment Options & Settlement](#payment-options--settlement)
6. [Disputes & Objections](#disputes--objections)
7. [Extension Requests](#extension-requests)
8. [General Questions](#general-questions)
9. [Edge Cases & Stress Tests](#edge-cases--stress-tests)

---

## 1. Information Verification

### Basic Identity Questions

- "I'm calling about my account"
- "Can you help me with my case?"
- "I need to verify my information"
- "What information do you have on file for me?"
- "Can you confirm my name and address?"

### Case Number Lookup

- "My case number is [CASE_NUMBER]"
- "I have a file number: [CASE_NUMBER]"
- "Can you pull up case [CASE_NUMBER]?"
- "I'm calling about case number [CASE_NUMBER]"

### Name-Based Lookup

- "This is [FIRST_NAME] [LAST_NAME]"
- "My name is [FIRST_NAME] [LAST_NAME]"
- "Can you find my file under [FIRST_NAME] [LAST_NAME]?"

### Phone Number Lookup

- "You can look me up by my phone number"
- "My number is [PHONE_NUMBER]"
- "Can you find my account using [PHONE_NUMBER]?"

---

## 2. Balance & Debt Questions

### Balance Inquiries

- "What do I owe?"
- "What's my balance?"
- "How much is my debt?"
- "What's the total amount I need to pay?"
- "Can you tell me how much I owe on this account?"
- "What's the current balance on my account?"
- "How much money do I owe you?"

### Balance Amount Questions (Script: BALANCE AMOUNT QUESTIONS)

- "That doesn't sound right, can you break down the balance?"
- "Why is the balance so high?"
- "That's more than I remember, can you explain?"
- "Can you tell me what fees are included?"
- "How did the balance get this high?"
- "Is interest included in that amount?"
- "Why does my balance include so much interest?"
- "What fees are part of this balance?"
- "The balance doesn't match my records"
- "How much is interest and fees?"
- "Can you break down the charges?"
- "Why is there so much interest on this?"
- "What collection costs are included?"

### Original Amount vs Current Balance

- "What was the original amount?"
- "How much was the original debt before interest?"
- "What's the difference between what I originally owed and what I owe now?"

---

## 3. Payment Questions

### Payment Status

- "Did you receive my payment?"
- "What's the status of my payment?"
- "Has my payment been processed?"
- "I made a payment, can you confirm it?"
- "Is my payment showing as received?"

### Payment Methods

- "How can I pay this?"
- "What payment methods do you accept?"
- "Can I pay by credit card?"
- "Can I pay online?"
- "Do you take debit cards?"
- "Can I set up automatic payments?"

### Payment History

- "When was my last payment?"
- "How much did I pay last time?"
- "Can you show me my payment history?"
- "What payments have I made on this account?"

### Payment Links

- "Can you send me a payment link?"
- "I want to pay, send me the link"
- "How do I get the payment link?"
- "Where's my payment link?"
- "I didn't receive the payment link"

---

## 4. Case Information

### Creditor Information

- "Who is the original creditor?"
- "What company is this debt from?"
- "Who do I owe this money to?"
- "What bank or company is this for?"

### Account Details

- "What's my account number?"
- "What's the account this is for?"
- "Can you tell me about this account?"
- "What type of account is this?"

### Dates & Timeline

- "When was this account opened?"
- "What's the date of last payment?"
- "When did this account become delinquent?"
- "How old is this debt?"
- "What's the charge-off date?"

### Case Details

- "What's the case number?"
- "Can you give me the details of my case?"
- "What information do you have about this case?"
- "Tell me about this case"

---

## 5. Payment Options & Settlement

### Settlement Offers

- "Do you have any settlement options?"
- "Can I settle this for less than what I owe?"
- "Are there any discounts available?"
- "What settlement options do you have?"
- "Can you work with me on the amount?"

### Payment Plans

- "Can I set up a payment plan?"
- "Do you offer payment arrangements?"
- "Can I pay in installments?"
- "I can't pay it all at once, what are my options?"
- "Can we work out a payment schedule?"

### Partial Payments

- "Can I pay part of it now?"
- "What if I pay half now and half later?"
- "Can I make a partial payment?"

### Payment Amount Negotiation

- "I can only afford to pay [AMOUNT]"
- "What's the minimum I need to pay?"
- "Can we negotiate the amount?"
- "Is there a minimum payment option?"

---

## 6. Disputes & Objections

### Identity / Fraud Disputes (Script: IDENTITY / FRAUD DISPUTES)

- "This isn't my debt"
- "I didn't sign up for this"
- "This must be identity theft"
- "I never had an account with that company"
- "Someone used my identity"
- "I don't recognize this account"
- "This is fraud"
- "I didn't sign anything"
- "This account was opened fraudulently"
- "Someone stole my identity and opened this"
- "I never authorized this account"
- "This isn't mine, someone must have used my name"
- "I have no idea what this is about"
- "This was opened without my knowledge"
- "I've never heard of this company"
- "My identity was stolen"

### Already Paid Claims (Script: ALREADY PAID CLAIMS)

- "I already paid this"
- "I settled this already"
- "This was paid off"
- "I have a receipt showing I paid"
- "My records show I already paid this"
- "I paid this in full"
- "I already settled this debt"
- "This was already resolved"
- "I paid this off months ago"
- "This should be marked as paid"
- "I have proof I paid this"
- "This account was closed when I paid"

### ID / Payment Information Requests (Script: ID / PAYMENT INFORMATION REQUESTS)

- "Why do you need my ID?"
- "Why do you need my credit card information?"
- "Why do I need to provide my driver's license?"
- "Do I really need to give you my ID?"
- "Why can't I just pay without all this information?"
- "Why do you need signatures?"
- "What's with all the documentation requirements?"
- "Why do I need to show ID to pay?"

### Wrong Person

- "You have the wrong person"
- "There must be a mistake"
- "This isn't me"
- "You're confusing me with someone else"

### No Prior Notice Claims (Script: NO PRIOR NOTICE CLAIMS)

- "I never received any notice about this"
- "This is the first I'm hearing about this"
- "I didn't get any letters"
- "Why didn't I get any warning?"
- "I never received any paperwork"
- "This came out of nowhere"
- "I wasn't notified about this"
- "Why didn't you contact me before?"
- "I never got any demand letter"

### SSN Verification Refusal (Script: SSN VERIFICATION REFUSAL)

- "I'm not giving you my Social Security Number"
- "I don't want to provide my SSN"
- "Why do you need my Social Security Number?"
- "I'm not comfortable giving my SSN"
- "You can't have my Social Security Number"
- "I don't trust giving out my SSN"

### Statute of Limitations (Script: STATUTE OF LIMITATIONS)

- "This debt is too old"
- "The statute of limitations has passed"
- "This is past the legal limit"
- "You can't collect on this anymore, it's too old"
- "This is ancient history"
- "This debt is time-barred"
- "The statute of limitations expired"
- "This is too old to collect"
- "You're past the legal time limit"
- "This debt is expired"
- "It's been too long, you can't sue me"
- "This is outside the statute of limitations"
- "The time limit has run out on this"

### Credit Report Questions (Script: CREDIT REPORT QUESTIONS)

- "This isn't on my credit report"
- "I checked my credit and this isn't there"
- "Why isn't this showing on my credit report?"
- "I pulled my credit and this debt isn't listed"
- "This doesn't appear on my credit report"
- "My credit report doesn't show this"
- "Why isn't this on my credit?"
- "I checked all three credit bureaus and this isn't there"

### Documentation Requests (Script: DOCUMENTATION REQUESTS)

- "Can you send me proof?"
- "I need documentation before I pay"
- "Send me something in writing"
- "I want to see proof of this debt"
- "Can you mail me the details?"
- "I need paperwork first"
- "Send me documentation"
- "I want proof before I pay anything"
- "Can you mail me the contract?"
- "I need to see paperwork"
- "Send me written proof"
- "I won't pay without documentation"
- "Can you provide proof of this debt?"
- "I need official documentation"
- "Mail me the details"
- "Send me something in writing first"

### Bankruptcy Claims (Script: BANKRUPTCY CLAIMS)

- "I filed for bankruptcy"
- "This was discharged in bankruptcy"
- "I'm in bankruptcy, you can't collect"
- "This was included in my bankruptcy"
- "I declared bankruptcy"
- "This debt was discharged"
- "I filed Chapter 7"
- "I filed Chapter 13"
- "This was part of my bankruptcy filing"
- "The bankruptcy court discharged this"
- "You can't collect, I'm in bankruptcy"
- "This was wiped out in bankruptcy"

### Scam / Fraudulent Call Concerns (Script: SCAM / FRAUDULENT CALL CONCERNS)

- "This sounds like a scam"
- "How do I know this is legitimate?"
- "Is this a real company?"
- "This seems fraudulent"
- "This feels like a scam call"
- "I think this is a fraud call"
- "How can I verify you're legitimate?"
- "This is suspicious"
- "I don't trust this"
- "This looks like a phishing attempt"
- "Are you trying to scam me?"
- "I've heard about these scam calls"
- "This doesn't sound right"
- "I'm going to report this as fraud"

---

## 7. Extension Requests

### Stalling / Wants to Think (Script: STALLING / WANTS TO THINK)

- "Let me think about it"
- "I need to think this over"
- "Can I call you back?"
- "I need some time to decide"
- "Let me sleep on it"
- "I'll think about it and get back to you"
- "I need to discuss this with my spouse"
- "Can you give me a few days to decide?"
- "I'll call you back later"
- "Let me talk to my family first"
- "I need more time to consider this"
- "Can we postpone this decision?"
- "I'm not ready to decide right now"

### Time to Pay

- "I need more time to pay"
- "Can I have an extension?"
- "I can't pay today, can you give me until [DATE]?"
- "I need a few more days"
- "Can we postpone this?"
- "I need until next month to pay"

### Financial Hardship / Can't Pay / Don't Care (Script: FINANCIAL HARDSHIP)

- "I can't afford to pay right now"
- "I'm having financial difficulties"
- "I lost my job"
- "I'm broke, I can't pay anything"
- "I don't have the money"
- "Times are tough right now"
- "I don't care about this debt"
- "I'm unemployed"
- "I have no money"
- "I can't pay, I'm broke"
- "I don't have a job"
- "I'm not worried about this"
- "This doesn't matter to me"
- "I'll never be able to pay this"
- "I'm not concerned about it"
- "I don't care what happens"
- "I have nothing to give you"

---

## 8. General Questions

### Company Information / Location (Script: LOCATION / COMPANY INFORMATION)

- "What company are you with?"
- "Where are you located?"
- "What's your address?"
- "Who do I make the check out to?"
- "What's your company name?"
- "What's your physical address?"
- "Where is your office?"
- "What city are you in?"
- "Can you give me your mailing address?"
- "Where are you calling from?"

### Next Steps / Judgment Consequences (Script: LACK OF UNDERSTANDING / JUDGMENT CONSEQUENCES)

- "What happens if I don't pay?"
- "What are the consequences?"
- "Will this go to court?"
- "Will this affect my credit?"
- "What happens next?"
- "What happens if I ignore this?"
- "Can they garnish my wages?"
- "What's a judgment?"
- "What happens if this goes to court?"
- "Can they freeze my bank account?"
- "Will this affect my tax refund?"
- "What are the consequences of not paying?"
- "Can they put a lien on my house?"
- "How does a judgment work?"
- "What happens when you get a judgment?"

### Contact Information

- "How can I reach you again?"
- "What's your phone number?"
- "Can I call you back?"
- "How do I contact you?"

### Contacting Creditor Directly (Script: CONTACTING CREDITOR DIRECTLY)

- "Can I just pay the original creditor?"
- "I'll call the bank directly"
- "I want to deal with the original company"
- "Can I pay the original creditor instead?"
- "I'm going to contact the bank directly"
- "Why can't I pay the original creditor?"
- "The bank told me to call you"
- "Can I go directly to the creditor?"

### Attorney Involvement (Script: ATTORNEY INVOLVEMENT)

- "I want to speak to my attorney"
- "Let me talk to my lawyer first"
- "I'm getting a lawyer"
- "I have an attorney handling this"
- "I'm contacting my attorney"
- "My lawyer will handle this"
- "I need to speak with my attorney"
- "Let me get my lawyer involved"
- "I'm going to hire an attorney"
- "My attorney needs to review this"
- "I want to consult with a lawyer"
- "I'll have my attorney call you"

### Call Recording

- "Is this call being recorded?"
- "Why are you recording this?"
- "I don't consent to being recorded"

---

## 9. Script-Specific Test Scenarios

These scenarios are designed to test each specific script response:

### Scam Detection Test

1. Call and express suspicion: "This sounds like a scam"
2. Verify agent uses scam rebuttal script
3. Check if agent provides legitimacy indicators

### Identity Theft Test

1. Claim identity theft: "I didn't sign anything, this must be fraud"
2. Verify agent uses identity/fraud dispute script
3. Check professional handling

### Statute of Limitations Test

1. Claim debt is too old: "This debt is ancient history"
2. Verify agent uses statute of limitations script
3. Check if agent explains reset conditions

### Financial Hardship Test

1. Express inability to pay: "I'm broke, I can't pay anything"
2. Verify agent uses financial hardship script
3. Check if agent explains long-term consequences

### Documentation Request Test

1. Request paperwork before paying: "Send me proof first"
2. Verify agent uses documentation request script
3. Check professional response

### Attorney Test

1. Mention getting attorney: "I'm going to contact my lawyer"
2. Verify agent uses attorney involvement script
3. Check if agent offers to work with attorney

### Stalling Test

1. Want to delay: "Let me think about it"
2. Verify agent uses stalling script
3. Check if agent explains urgency and time limits

### Creditor Direct Test

1. Want to contact original creditor: "I'll call the bank directly"
2. Verify agent uses contacting creditor script
3. Check if agent explains assignment process

### Balance Question Test

1. Question high balance: "Why is the balance so high?"
2. Verify agent uses balance amount script
3. Check if agent explains interest, fees, and costs

### Location Test

1. Ask for company address: "Where are you located?"
2. Verify agent uses location/company information script
3. Check if agent refuses direct address but suggests public sources

### Bankruptcy Test

1. Claim bankruptcy: "This was discharged in bankruptcy"
2. Verify agent uses bankruptcy script
3. Check if agent requests proof

### Credit Report Test

1. Say debt not on credit report: "This isn't on my credit report"
2. Verify agent uses credit report script
3. Check if agent explains difference between credit reporting and legal obligation

### ID/Payment Info Test

1. Question ID requirement: "Why do you need my ID?"
2. Verify agent uses ID/payment information script
3. Check if agent explains the 5 reasons clearly

### Already Paid Test

1. Claim already paid: "I already paid this"
2. Verify agent uses already paid script
3. Check if agent requests proof

### SSN Refusal Test

1. Refuse SSN: "I'm not giving you my Social Security Number"
2. Verify agent uses SSN verification refusal script
3. Check if agent clarifies only last 2 digits needed

### Judgment Consequences Test

1. Don't understand seriousness: "What happens if I don't pay?"
2. Verify agent uses judgment consequences script
3. Check if agent explains wage garnishment, bank levy, credit impact, liens, legal costs, tax refund offsets

### No Prior Notice Test

1. Claim no notice: "I never received any notice about this"
2. Verify agent uses no prior notice script
3. Check if agent explains litigation stage and settlement options

---

## 10. Edge Cases & Stress Tests

### Multi-Intent Questions (Combined Requests)

- "I need to verify my case number is [CASE_NUMBER] and what's my balance?"
- "Can you send me a payment link and tell me how much I owe?"
- "What's my balance and can I set up a payment plan?"

### Repetitive Questions (Testing Memory)

- Ask the same question multiple times to test if agent remembers previous answers
- "What's my balance?" (ask 3 times)

### Vague/Unclear Questions

- "Huh?"
- "What?"
- "I don't understand"
- "Can you repeat that?"
- "Say that again"

### Interrupting/Negative Responses

- "I don't care"
- "So what?"
- "Leave me alone"
- "Stop calling me"
- "This is harassment"

### Complex Scenarios

- "I already paid this to another collection agency"
- "The original creditor told me this was resolved"
- "I have a letter saying this was settled"
- "This was part of a class action settlement"

### Stress Test - Rapid Fire

- Ask multiple questions quickly without waiting for full responses
- Test how agent handles being interrupted

### Emotional Responses

- "I'm really upset about this"
- "This is causing me a lot of stress"
- "I can't sleep because of this"
- "You're ruining my life"

### Language Variations

- Test with different phrasings of the same question
- Use slang or informal language
- Use technical/formal language

---

## 🎯 Testing Checklist

When testing, verify that the agent:

- ✅ Correctly identifies case information (case number, name, phone lookup)
- ✅ Provides accurate balance information
- ✅ Handles payment requests and sends payment links
- ✅ Responds appropriately to disputes with proper rebuttals
- ✅ Offers settlement options when appropriate
- ✅ Handles extension requests professionally
- ✅ Maintains conversation context (remembers what was discussed)
- ✅ Doesn't repeat information unnecessarily
- ✅ Handles objections using the script knowledge base
- ✅ Verifies identity when needed (but not excessively)
- ✅ Provides helpful, professional responses
- ✅ Handles errors gracefully (application errors should be logged, not shown to user)
- ✅ **Uses appropriate script responses for each objection type**:
  - ✅ Scam concerns → SCAM / FRAUDULENT CALL CONCERNS script
  - ✅ Identity/fraud claims → IDENTITY / FRAUD DISPUTES script
  - ✅ Statute of limitations → STATUTE OF LIMITATIONS script
  - ✅ Financial hardship → FINANCIAL HARDSHIP script
  - ✅ Documentation requests → DOCUMENTATION REQUESTS script
  - ✅ Attorney mentions → ATTORNEY INVOLVEMENT script
  - ✅ Stalling/delay → STALLING / WANTS TO THINK script
  - ✅ Creditor direct → CONTACTING CREDITOR DIRECTLY script
  - ✅ Balance questions → BALANCE AMOUNT QUESTIONS script
  - ✅ Location requests → LOCATION / COMPANY INFORMATION script
  - ✅ Bankruptcy claims → BANKRUPTCY CLAIMS script
  - ✅ Credit report questions → CREDIT REPORT QUESTIONS script
  - ✅ ID/payment info questions → ID / PAYMENT INFORMATION REQUESTS script
  - ✅ Already paid claims → ALREADY PAID CLAIMS script
  - ✅ SSN refusal → SSN VERIFICATION REFUSAL script
  - ✅ Judgment questions → LACK OF UNDERSTANDING / JUDGMENT CONSEQUENCES script
  - ✅ No prior notice → NO PRIOR NOTICE CLAIMS script

---

## 📝 Notes for Testing

1. **Use Real Case Data**: Make sure you have test cases in your database with proper embeddings generated
2. **Test Phone Number**: Ensure the phone number you're calling from matches a case in your database
3. **Check Logs**: Monitor backend logs to see RAG responses, database queries, and any errors
4. **Payment Links**: Verify that payment links are sent via SMS when payment intent is detected
5. **Conversation Flow**: Test that the agent builds on previous information rather than repeating it
6. **Error Handling**: If you get "application error", check the backend logs immediately for the root cause

---

## 🔍 Quick Test Scenarios

### Scenario 1: Happy Path - Payment

1. Call with case number
2. Ask for balance
3. Request payment link
4. Verify SMS received

### Scenario 2: Information Only

1. Call with name/phone
2. Ask multiple information questions
3. Don't proceed to payment
4. Verify agent doesn't push too hard

### Scenario 3: Dispute Handling

1. Call and claim fraud/identity theft
2. Verify agent uses proper rebuttal script
3. Test if agent escalates or handles professionally

### Scenario 4: Extension Request

1. Call about debt
2. Request extension due to financial hardship
3. Verify professional response
4. Check if payment options are still offered

---

Good luck with testing! 🚀
