# Learning Plan Modal – Resume Skill Gap Analyzer

A dynamic, phase-based **Learning Plan Modal** built using **React + TypeScript (TSX)**.  
This component helps users bridge skill gaps by generating a **structured, time-bound learning roadmap** based on missing and matched skills for a job role.

---

## 🚀 Features

- 📊 Automatic skill prioritization (**High / Medium / Low**)
- 🗓️ Estimated learning duration (in weeks)
- 📈 Highlights **high-demand skills**
- 🧩 Phase-wise roadmap (Critical → Core → Optional)
- 🔗 Direct external learning resources
- 🎯 Resume-oriented learning strategy
- 🧠 Practical learning tips included

---

## 🛠️ Tech Stack

- **React**
- **TypeScript (.tsx)**
- **ShadCN UI**
- **Tailwind CSS**
- **Lucide Icons**

---

## 📂 Component Overview

### `LearningPlanModal.tsx`

This component renders a modal dialog that:
- Accepts missing skills and matched skills as props
- Groups skills into learning phases
- Calculates total learning time
- Displays actionable learning steps
- Encourages systematic upskilling

---

## 📥 Props Interface

```ts
interface LearningPlanModalProps {
  open: boolean
  onOpenChange: (open: boolean) => void
  missingSkills: MissingSkill[]
  matchedSkills: MatchedSkill[]
}
