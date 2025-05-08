 # HR Employee Attrition Tracker 📊

This Excel-based HR tracker helps monitor employee attrition using:

- ✅ Tenure calculation (DATEDIF)
- ✅ Exit month (TEXT)
- ✅ VLOOKUP for department head mapping
- ✅ Pivot table to count attrition by status
- ✅ Conditional formatting for notice period > 6 months

## Screenshots

![Pivot Table Summary](pivot_summary.png)

## Sample Formulas Used

```excel
=IF(B2<>"",DATEDIF(D2,IF(E2="",TODAY(),E2),"Y"),"")
=IF(E2<>"",TEXT(E2,"mmmm"),"")
=IF(F2="Resigned",IF(DATEDIF(TODAY(),G2,"M")>6,"Yes","No"),"")

