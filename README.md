# Supreme Court of the United States Research

Repository holding data related to my SCOTUS research project

## Variables
- voteId
-   identifier including caseId, docketId, caseIssuesId
dateDecision
- 
decisionType
usCite
- United States Reports citation
sctCite
- Supreme Court Reporter citation
ledCite
- Lawyers' Edition of the United States Reports citation
lexisCite
- LEXIS Citation
term
- year
naturalCourt
- natural court is a period during which no personnel change occurs
- codes when there is a shift in personnel
chief
- identifies the chief justice during whose tenure the case was decided
docket
- docket number that the Supreme Court has assigned to the case
caseName
- name of the case
dateArgument
- day, month, and year that the case was orally argued before the Court
petitioner
- provides detailed information about the identity of the petitioner
respondent
- provides detailed information about the identity of the respondent
jurisdiction
- manner in which the court takes jurisdiction (cert, appeal, bail, ...)
threeJudgeFdc
- variable will be checked if the case was heard by a three-judge federal district court (occasionally called “as specially constituted district court”)
caseOrigin
- the court in which the case originated
caseSource
- identifies the court whose decision the Supreme Court reviewed
lcDisagreement
- indicates that the Supreme Court's majority opinion mentioned that one or more of the members of the court whose decision the Supreme Court reviewed dissented
certReason
- reason for granting cert (federal court conflict, state court conflict, ...)
lcDisposition
- treatment the court whose decision the Supreme Court reviewed accorded the decision of the court it reviewed, drop since too simmilar to winningParty
lcDispositionDirection
- whether the decision of the court whose decision the Supreme Court reviewed was itself liberal or conservative
declarationUncon
- indicates that the Court either declared unconstitutional an act of Congress; a state or territorial statute, regulation, or constitutional provision; or a municipal or other local ordinance
caseDisposition
- treatment the Supreme Court accorded the court whose decision it reviewed is contained in this variable, drop since too simmilar to winningParty
caseDispositionUnusual
- signify that the Court made an unusual disposition of the cited case which does not match the coding scheme of the preceding variable
**partyWinning (response variable)**
- indicates whether the petitioning party emerged victorious
- 0: denied
- 1: affirmed
- 2: unclear (dropped from data since very infrequent and outside scope of research)
precedentAlteration
- if the majority opinion effectively says that the decision in this case "overruled" one or more of the Court's own precedents
voteUnclear
- votes in a case are those specified in the opinions
issue
- identifies the issue for each decision
issueArea
- separates the issues identified in issue variable into the following larger categories
decisionDirection
- ideological direction of the decision
decisionDirectionDissent
- if the dissent and majority are in opposite or the same direction
authorityDecision1
- specify the bases on which the Supreme Court rested its decision with regard to each legal provision that the Court considered in the case
lawType
- identify the constitutional provision(s), statute(s), or court rule(s) that the Court considered in the case, coded more broadly than lawSupp
lawSupp
- identify the constitutional provision(s), statute(s), or court rule(s) that the Court considered in the case
majOpinWriter
- identifies the author of the Court's opinion or judgment
majOpinAssigner
- identifies the assigner of the opinion or judgment of the Court
splitVote
-  indicates whether the vote variables (e.g., majVotes, minVotes) pertain to the vote on the first or second issue (or legal provision), drop since over 99 percent of the votes are on the first issue
majVotes
- specifies the number of justices voting in the majority
minVotes
- indicates the number of justices voting in dissent
