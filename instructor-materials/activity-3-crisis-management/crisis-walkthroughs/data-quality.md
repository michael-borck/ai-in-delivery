# Crisis #1: Data Quality Disaster

## When Your System Gives Wrong Answers

---

## The Scenario

**Week 1 of Live Pilot:**
- Your AI system launches
- Accuracy tests showed 85% success
- But suddenly: AI is giving customers wrong tracking numbers, outdated policies, conflicting info
- Root cause: Training data got corrupted (old product info mixed with new)
- Impact: Hundreds of customers affected over 5 days
- **You have 30 minutes to decide**

---

## Applying the Framework

### **DIAGNOSE**

**What happened?**
- AI giving wrong information due to corrupted training data
- Scope: ~1,000 customer queries over 5 days

**What caused it?**
- Training data wasn't validated before model training
- Old product information mixed with current data
- No quality gate caught it before launch

**Why it matters:**
- It's a data problem, not a design problem
- The model itself is fine; the data it learned from is bad
- Fixable, but requires 2-3 weeks of data cleaning + retraining

---

### **DECIDE**

**Your options:**

| Option | Timeline | Risk | Team Impact |
|--------|----------|------|-------------|
| **Full Pause** | 2-3 weeks to fix | Medium (lose momentum) | Clear responsibility |
| **Hybrid Approach** | 2-3 weeks + ongoing QA | Medium (team overloaded) | Shared responsibility |
| **Continue + Enhanced QA** | 5-7 days if retraining works | HIGH (risky if timeline slips) | Heavy burden |
| **Kill Project** | Immediate | High (lose credibility) | Demoralising |

**Recommended: Full Pause**
- Stop all AI responses immediately
- Route all queries back to humans
- Spend 2-3 weeks cleaning data and retraining
- Restart with corrected system

**Why?** Safety first. A few weeks of delay is better than days of bad data damaging customer trust.

---

### **COMMUNICATE**

**To your team (immediate):**
> "We found a data quality issue in the training data. We're pausing all AI responses effective now. All queries go back to you while we fix this. It'll take 2-3 weeks. Here's what I need from each of you..."

**To leadership (same day):**
> "We discovered a data quality issue affecting ~1,000 queries. This is exactly why we run pilots. We found it in a contained environment (30% of traffic) before it would have hit 100% of customers. We're pausing, fixing, and restarting in 3 weeks."

**To customers (same day):**
> "We're making improvements to ensure system accuracy. You may see slower responses while we improve. Your data is secure."

---

### **DOCUMENT**

**What to record:**
- Date discovered and scope of impact
- Root cause (corrupted data, no validation gate)
- Decision made (pause and retrain)
- Timeline (2-3 weeks)
- **Key learning:** Data quality matters more than model sophistication. Garbage in = garbage out.

**What to change next time:**
- Add data validation step before model training
- Implement real-time accuracy monitoring in production
- Have clear pause/restart procedures documented

---

## Key Insights

**This teaches you:**
- Pilots exist to find these problems early
- Technical crises need fast diagnosis + clear decisions
- Crisis communication matters more than the crisis itself
- Recovery time is shorter than the damage of continued problems

**The big win:**
You found a major issue at 30% scale. If you'd scaled to 100% first, this would have been a catastrophe. That's why pilots work.

---

## Takeaway

When data quality fails:
1. **Diagnose immediately** (what corrupted, how many affected)
2. **Decide fast** (pause and fix vs. continue with controls)
3. **Communicate clearly** (team → leadership → customers)
4. **Document the learning** (so this doesn't happen again)

This is textbook crisis leadership: **clarity > speed**.
