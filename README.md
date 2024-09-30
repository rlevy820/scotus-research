# Supreme Court of the United States Research

Repository holding data related to my SCOTUS research project

## Variables
1. voteId
- identifier including caseId, docketId, caseIssuesId
2. dateDecision
- year, month, and day that the Court announced its decision in the case
3. decisionType
- type of decision (orally argued, no oral argument, decrees, ...)
4. usCite
- United States Reports citation
5. sctCite
- Supreme Court Reporter citation
6. ledCite
- Lawyers' Edition of the United States Reports citation
7. lexisCite
- LEXIS Citation
8. term
- year
9. naturalCourt
- natural court is a period during which no personnel change occurs
- codes when there is a shift in personnel
10. chief
- identifies the chief justice during whose tenure the case was decided
11. docket
- docket number that the Supreme Court has assigned to the case
12. caseName
- name of the case
13. dateArgument
- day, month, and year that the case was orally argued before the Court
14. petitioner
- provides detailed information about the identity of the petitioner
15. respondent
- provides detailed information about the identity of the respondent
16. jurisdiction
- manner in which the court takes jurisdiction (cert, appeal, bail, ...)
17. threeJudgeFdc
- variable will be checked if the case was heard by a three-judge federal district court (occasionally called “as specially constituted district court”)
18. caseOrigin
- the court in which the case originated
19. caseSource
- identifies the court whose decision the Supreme Court reviewed
20. lcDisagreement
- indicates that the Supreme Court's majority opinion mentioned that one or more of the members of the court whose decision the Supreme Court reviewed dissented
21. certReason
- reason for granting cert (federal court conflict, state court conflict, ...)
22. lcDisposition
- treatment the court whose decision the Supreme Court reviewed accorded the decision of the court it reviewed, drop since too simmilar to winningParty
23. lcDispositionDirection
- whether the decision of the court whose decision the Supreme Court reviewed was itself liberal or conservative
24. declarationUncon
- indicates that the Court either declared unconstitutional an act of Congress; a state or territorial statute, regulation, or constitutional provision; or a municipal or other local ordinance
25. caseDisposition
- treatment the Supreme Court accorded the court whose decision it reviewed is contained in this variable, drop since too simmilar to winningParty
26. caseDispositionUnusual
- signify that the Court made an unusual disposition of the cited case which does not match the coding scheme of the preceding variable
27. **partyWinning (response variable)**
- indicates whether the petitioning party emerged victorious
- 0: denied
- 1: affirmed
- 2: unclear (dropped from data since very infrequent and outside scope of research)
28. precedentAlteration
- if the majority opinion effectively says that the decision in this case "overruled" one or more of the Court's own precedents
29. voteUnclear
- votes in a case are those specified in the opinions
30. issue
- identifies the issue for each decision
31. issueArea
- separates the issues identified in issue variable into the following larger categories
32. decisionDirection
- ideological direction of the decision
33. decisionDirectionDissent
- if the dissent and majority are in opposite or the same direction
34. authorityDecision1
- specify the bases on which the Supreme Court rested its decision with regard to each legal provision that the Court considered in the case
35. lawType
- identify the constitutional provision(s), statute(s), or court rule(s) that the Court considered in the case, coded more broadly than lawSupp
36. lawSupp
- identify the constitutional provision(s), statute(s), or court rule(s) that the Court considered in the case
37. majOpinWriter
- identifies the author of the Court's opinion or judgment
38. majOpinAssigner
- identifies the assigner of the opinion or judgment of the Court
39. splitVote
-  indicates whether the vote variables (e.g., majVotes, minVotes) pertain to the vote on the first or second issue (or legal provision), drop since over 99 percent of the votes are on the first issue
40. majVotes
- specifies the number of justices voting in the majority
41. minVotes
- indicates the number of justices voting in dissent
