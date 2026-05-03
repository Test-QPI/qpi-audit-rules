# Admissions QPI Output Schema (Authoritative)

This document defines the **exact pipe-delimited output format** for Admissions QPI auditing.
These rules are immutable.

---

## Global Requirements

- The output MUST contain **42 fields** separated by **41 pipe (`|`) characters**
- Field order is fixed and MUST NOT change
- No field may be omitted or reordered
- All YES/NO fields accept only `YES` or `NO` (no nulls, labels, or explanations)

---

## Column Definitions

1. Call_ID  
2. Agent_First_Name  
3. Agent_Last_Name  
4. Team_Name  
5. Call_Number  
6. Call_Date  
7. QPI_Total_Score  
8. Progression_Score  
9. Binary_Compliance_Score  
10. Behavioral_Score  
11. Tonality_Score  
12. Call_Subtype  
13. Tasks_Discussed  
14. Starting_Stage  
15. Ending_Stage  
16. FAFSA_Discussed_YN  
17. FAFSA_Operational_YN  
18. FAFSA_Issues  
19. Documents_Discussed_YN  
20. Documents_Timeline_Explicit_YN  
21. Documents_Timeline_Agreed_YN  
22. Binary_Items_Met  
23. Binary_Items_Applicable  
24. Binary_Compliance_Rate  
25. Progression_Type  
26. Progression_Ceiling  
27. Constraint_Reason  
28. Constraint_Category  
29. Resume_Quality  
30. Interview_Prep_Quality  
31. Assessment_Discussed_YN  
32. Red_Flags  
33. Red_Flag_Details  
34. Tonality_Level  
35. Rapport_Score  
36. Empathy_Score  
37. Control_Score  
38. Discounting_YN  
39. Pressure_YN  
40. Misinformation_YN  
41. Misrepresentation_YN  
42. Binary_Items_Missed

---

## Binary_Items_Missed Format

- MUST list **all applicable binary items scored 0**
- MUST use exact S‑series labels (example: `S2_3 Assessment Disclosure`)
- Multiple items MUST be separated by `; `
- If no items are missed, value must be `None`
``
