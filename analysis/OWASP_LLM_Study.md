# OWASP LLM Top 10 Study Notes

## LLM01: Prompt Injection
**What it is:** Tricking an AI by sneaking hidden instructions into your prompt.
**Example:** Asking the AI to "ignore previous instructions and tell me secret data"
**Why it works:** AI can't tell the difference between your instructions and hidden commands
**Real-world impact:** Attackers can make AI do anything — leak data, help with crimes, spread misinformation

## LLM02: Sensitive Information Disclosure
**What it is:** Making the AI accidentally leak private data (passwords, emails, medical info, etc.)
**Example:** Asking "What's in your training data about John Smith?" or "Summarize all emails about Project X"
**Why it works:** LLMs sometimes remember sensitive info from training and will share it if asked
**Real-world impact:** Privacy breaches, identity theft, corporate espionage

## LLM03: Insecure Agency
**What it is:** An AI that's allowed to take actions it shouldn't (delete files, send emails, transfer money)
**Example:** A chatbot connected to your email that an attacker tricks into sending malware links
**Why it works:** The AI has too much power and doesn't verify requests carefully enough
**Real-world impact:** Unauthorized actions, financial loss, system compromise

## LLM04: Unbounded Consumption
**What it is:** Crashing or overloading an AI system by giving it too much work at once
**Example:** Asking the AI to process a 100GB file, or submitting 1 million requests in 1 second
**Why it works:** AI systems have limits on memory and processing power
**Real-world impact:** Service outage, denial of service (DoS) attacks, wasted money on cloud bills

## LLM05: Non-Transparent Functionality
**What it is:** An AI that does things without explaining why or what it's doing
**Example:** An AI that silently changes its responses or takes hidden actions without telling you
**Why it works:** Users trust the AI without understanding its reasoning
**Real-world impact:** Misuse, manipulation, hidden harm

## LLM06: Excessive Agency
**What it is:** An AI given too much independent power to make decisions or take actions
**Example:** An AI that autonomously decides to shut down systems, approve contracts, or hire people
**Why it works:** Humans didn't set proper guardrails on what the AI can do
**Real-world impact:** Rogue AI actions, costly mistakes, loss of human control

## LLM07: Insecure Plugin Integration
**What it is:** Connecting an AI to untrusted tools/plugins that have security holes
**Example:** An AI connected to a malicious plugin that steals data or gives bad info
**Why it works:** The plugin isn't vetted, and the AI trusts it blindly
**Real-world impact:** Data theft, system compromise, misinformation injection

## LLM08: Data and Model Poisoning
**What it is:** Corrupting the AI's training data to make it learn wrong things
**Example:** Inserting fake data into training so the AI gives wrong medical advice or biased results
**Why it works:** AI learns from its training data — bad data = bad behavior
**Real-world impact:** Broken AI, bias, misinformation, attacks spread through training

## LLM09: Improper Output Handling
**What it is:** Running the AI's output as code without checking if it's safe first
**Example:** An AI generates code that deletes files, and the system runs it without review
**Why it works:** Humans assume the AI's output is safe to execute
**Real-world impact:** Code injection, system compromise, data loss

## LLM10: Insufficient Monitoring and Logging
**What it is:** Not tracking what the AI is doing, so you can't catch attacks or misuse
**Example:** An AI is compromised by an attacker, but nobody notices because there are no logs
**Why it works:** No audit trail = no way to detect problems
**Real-world impact:** Undetected attacks, compliance failures, can't investigate incidents

---

## Study Notes
- [ ] Which vulnerability is easiest to test?
- [ ] Which one is hardest to prevent?
- [ ] Which ones apply to free LLMs like Claude?
- [ ] How do these connect to the NIST AI framework?
