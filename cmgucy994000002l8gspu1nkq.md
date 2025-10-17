---
title: "01 Bug, Error, and Defect"
datePublished: Fri Oct 17 2025 04:37:46 GMT+0000 (Coordinated Universal Time)
cuid: cmgucy994000002l8gspu1nkq
slug: 01-bug-error-and-defect
tags: shreenibas

---

**Bug**, **Error**, and **Defect** in software testing. Many people use them interchangeably, but they have subtle differences:

---

## **1\. Error**

* **Definition:** A **mistake made by a developer** while coding or designing the software.
    
* **Nature:** Human mistake.
    
* **Example:** A programmer writes `if(a = 5)` instead of `if(a == 5)` in Java.
    
* **When it occurs:** During **coding or design** phase.
    
* **Key Point:** Errors are **not directly visible to end-users** until they lead to a defect.
    

---

## **2\. Defect**

* **Definition:** A **flaw or imperfection in the software** that may cause the software to behave unexpectedly.
    
* **Nature:** Found in the **developed software**.
    
* **Example:** Login button doesn’t respond when clicked.
    
* **When it occurs:** After coding, usually **found during testing**.
    
* **Key Point:** Defects are often caused by **errors in code or design**.
    

---

## **3\. Bug**

* **Definition:** Another name for a **defect**; a bug is a defect that is **reported by testers** and tracked in a bug tracking tool.
    
* **Nature:** Detected issue in the software that needs fixing.
    
* **Example:** A tester finds that the login page crashes for a specific username and logs it in Jira as a bug.
    
* **Key Point:** A bug is a **defect identified and documented**.
    

---

### **Summary Table**

| Term | Cause | Where Found | Example |
| --- | --- | --- | --- |
| **Error** | Human mistake | Code/Design | `if(a = 5)` instead of `if(a == 5)` |
| **Defect** | Mistake in software | Testing phase | Login button doesn’t work |
| **Bug** | Defect reported | Bug tracking tool | Tester logs login crash in Jira |

---

💡 **Key point:**

* **Error → Defect → Bug** is like a chain:  
    Developer makes an **error** → leads to a **defect** in software → Tester logs it as a **bug**.
    

---

If you want, I can also draw a **simple diagram showing the relationship between Error, Defect, and Bug** which makes it easier to remember.

Do you want me to create that diagram?

##### You said:

Severity priority in detail

###### ChatGPT said:

Here’s a **detailed explanation of Severity and Priority** in software testing, including their differences, examples, and use in bug management:

---

## **1\. Severity**

* **Definition:** Severity defines the **impact of a bug on the application or system**. It tells how serious the defect is from a **technical perspective**.
    
* **Controlled by:** Tester / QA team
    
* **Focus:** **Business or application impact**, not urgency
    
* **Categories:**
    

| Severity Level | Description | Example |
| --- | --- | --- |
| **Critical / Showstopper** | Bug causes system crash, data loss, or prevents use of the application | Login page crashes for all users |
| **Major / High** | Bug affects major functionality but system still works partially | Payment not processed in e-commerce site |
| **Medium / Moderate** | Bug affects non-critical functionality | Incorrect calculation in reports |
| **Low / Minor** | Cosmetic issues, UI glitches, spelling mistakes | Misaligned text, color issue |
| **Trivial / Suggestion** | No real impact; enhancement or improvement | Tooltip text missing |

💡 **Key point:** Severity = **how serious the problem is**.

---

## **2\. Priority**

* **Definition:** Priority defines the **order in which a bug should be fixed**. It tells **how urgently a defect must be resolved**.
    
* **Controlled by:** Product Owner / Project Manager
    
* **Focus:** **Business urgency**, deadlines, release impact
    
* **Categories:**
    

| Priority Level | Description | Example |
| --- | --- | --- |
| **High / P1 / Urgent** | Must fix immediately; release cannot proceed without this | Login failure for all users |
| **Medium / P2 / Normal** | Important but can wait for next patch | Search function slow for large data |
| **Low / P3 / Minor** | Can be fixed in future release | Color mismatch in button on rarely used page |

💡 **Key point:** Priority = **how quickly it should be fixed**.

---

## **3\. Difference Between Severity and Priority**

| Aspect | Severity | Priority |
| --- | --- | --- |
| **Definition** | Impact of defect on system | Urgency of fixing the defect |
| **Controlled by** | Tester / QA | Project Manager / Product Owner |
| **Focus** | Technical/business impact | Business release schedule |
| **Example** | App crashes → Critical | Cosmetic issue → Low priority |
| **Independent?** | Can be independent of priority | Can be independent of severity |

---

### **4\. Examples for Better Understanding**

| Bug Scenario | Severity | Priority | Reason |
| --- | --- | --- | --- |
| Login page crashes for all users | Critical | High | System unusable, urgent fix |
| Misspelled text in homepage header | Low | Medium | Minor issue but visible to users |
| Report calculation wrong but workaround exists | Major | Medium | Important, not urgent |
| Button color misaligned on rarely used page | Minor | Low | Cosmetic, can wait |

---

💡 **Tip for QA / Testing Interviews:**

* Severity = **How bad is it?**
    
* Priority = **How fast should it be fixed?**
    

---

If you want, I can also make a **diagram showing severity vs priority matrix** which is very popular for interviews.

Do you want me to make that diagram?

##### You said:

Ok

###### ChatGPT said:

Perfect! Let’s visualize **Severity vs Priority** using a **matrix**, which is very common in QA interviews:

---

## **Severity-Priority Matrix**

| Severity \\ Priority | High Priority (P1) | Medium Priority (P2) | Low Priority (P3) |
| --- | --- | --- | --- |
| **Critical** | ✅ Must fix immediately | ❌ Rare, but may exist | ❌ Usually not applicable |
| **Major** | ✅ Important & urgent | ✅ Can be fixed in next release | ❌ Rarely |
| **Medium** | ✅ Could be urgent for specific cases | ✅ Normal fix schedule | ✅ Can be deferred |
| **Low / Minor** | ✅ Cosmetic but urgent for client | ✅ Can wait | ✅ No immediate impact |
| **Trivial** | ❌ Rarely | ✅ Can wait | ✅ Can be ignored |

---

### **How to Read the Matrix**

1. **Critical + High Priority (P1):** System crash or data loss → fix immediately.
    
2. **Major + Medium Priority (P2):** Major feature bug, but not blocking release → schedule fix.
    
3. **Low + Low Priority (P3):** Cosmetic UI issue → fix in future release.
    

💡 **Tip:** Severity is **vertical** (impact), Priority is **horizontal** (urgency).