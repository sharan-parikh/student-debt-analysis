# Possible features required in analyzing the student debt in USA.

## Category: Root

1. OPEID

## Category: About the Institution

1. INSTNM
2. ALIAS
3. Location
4. Main/Campus branch
5. Currently Operating
6. Title IV Eligibility Type, (OPEFLAG = 1, 2 and 3 only)
7. DISTANCEONLY (I think we should only take institutions that have DISTANCEONLY=FALSE)

## Category: Academics(Not Necessary, I think)

All category columns that start with **CIP**. (**0** means that the instituition **does not offer** that course and 1 means it **offers the course**)

## Category: Admissions

1. Open Admission Policy
2. Admission Rate

## Category: Costs

1. COSTT4_A (academic year institutions)
2. COSTT4_P (program-year institutions)
3. TUITIONFEE_IN - the cost data include the tuition and required fees, books
   and supplies, and living expenses estimated by the institution. Tuition
   and required fees are provided for in-district students
4. TUITIONFEE_OUT - same as TUITIONFEE_IN but for out-of-state students
5. TUITIONFEE_PROG - for program-year institutions
6. **_Average Net Price_** - The average annual cost of attendance includes tuition and fees, books
   and supplies, and living expenses for all full-time, first-time, degree-
   /certificate-seeking undergraduates who receive Title IV aid.

## Category: Students

1. UGDS - includes the number of degree/certificate-seeking undergraduates enrolled in the fall.
2. UGDS_MEN, UGDS_WOMEN, UGDS_WHITE, UGDS_BLACK, UGDS_HISP, UGDS_ASIAN, UGDS_AIAN, UGDS_NHPI, UGDS_2MOR, UGDS_NRA and UGDS_UNKN
3. NUM\[1-5\]\_\[PUB or PRIV\] - These elements report the number of full-time, first-time, degree/certificate-seeking undergraduates who received Title IV aid in each income bracket from the IPEDS Student Financial Aid (SFA) component.

## Category: Financial Aid

1. FTFTPCTFLOAN - shows the share of full-time, first-time
   degree/certificate-seeking undergraduate students who received
   federal loans in a given year

2. DEBT_MDN - This is the median loan debt accumulated at the institution by all
   student borrowers of federal loans who separate (i.e., either graduate
   or withdraw) in a given fiscal year, measured at the point of separation.

3. GRAD_DEBT_MDN - for students who completed
4. WDRAW_DEBT_MDN - for students who withdrew without completing
5. PLUS_DEBT_INST_MD

## Category: Repayment

1. CDR3
2. BBRR\[YR\]\_\[LOAN\]\_\[\GROUP]\_\[STATUS\] - ([YR]=1, 2, 3, or 4) after entering repayment.\
   Available **STATUS** values - **_Default, Delinquent, Forbearance, Deferment, Not making progress, Making progress, Paid in full, Discharged_**
3. DBRR\[YR\]\_\[LOAN\]\_\[GROUP]\_\[METRIC\] - ([YR]=1, 4, 5, 10, 20) after entering repayment
   **_[LOAN]=FED, [GROUP]=UG, UGCOMP, UGNOCOMP, UGUNK_**\
   This element depicts the outstanding balance (principal plus interest), amount originally disbursed, ratio of outstanding balance to amount disbursed, and number of borrowers at each institution who entered repayment at any point during a two-award-year period.
