{% from "_module-" + module + "/weeklyTpTasks.mbdf" import weekly_tp_themes with context %}

{% set admin_topics = [
  {level: 1, id: "moduleOverview", title: module_pair + ": " + module_name, link: "moduleOverview.html", alt: "Module Overview"},
  {level: 1, id: "usingThisWebsite", title: "Using this Website", link: "usingThisWebsite.html", highlight: "true", priority: 1},
  {level: 1, id: "moduleExpectations", title: "Module Expectations", link: "moduleExpectations.html", priority: 2},
  {level: 0, id: "moduleStructure", title: "Module Structure"},
    {level: 2, id: "weeklySchedule", title: "Weekly Schedule", link: "weeklySchedule.html", priority: 3},
    {level: 2, id: "lectures", title: "Lectures/Tutorials", link: "lectures.html", priority: 3},
  {level: 1, id: "instructors", title: "Instructors", link: "instructors.html", priority: 4},
  {level: 1, id: "textbooks", title: "Textbooks", link: "textbooks.html", priority: 2},
  {level: 1, id: "programmingLanguages", title: "Programming Language", link: "programmingLanguages.html", priority: 2},
  {level: 1, id: "standardsAndConventions", title: "Standards/Conventions", link: "standardsAndConventions.html", priority: 2},
  {level: -1, id: "ip", title: "Individual Project (iP)"},
    {level: 2, id: "ip-overview", title: "iP (Individual Project): Overview", link: "ip-overview.html", priority: 2},
    {level: 2, id: "ip-w2", title: "iP: Week 2", link: "ip-w2.html", priority: 2},
    {level: 2, id: "ip-w3", title: "iP: Week 3", link: "ip-w3.html", priority: 2},
    {level: 2, id: "ip-w4", title: "iP: Week 4", link: "ip-w4.html", priority: 2},
    {level: 2, id: "ip-w5", title: "iP: Week 5", link: "ip-w5.html", priority: 2},
    {level: 2, id: "ip-w6", title: "iP: Week 6", link: "ip-w6.html", priority: 1},
    {level: 2, id: "ip-grading", title: "iP: Grading", link: "ip-grading.html", priority: 2},
  {level: -1, id: "project", title: "Team Project (tP)"},
    {level: 2, id: "tp-expectations", title: "tP (team project): Expectations", link: "tp-expectations.html", priority: 2},
    {level: 2, id: "tp-timeline", title: "tP: Timeline", link: "tp-timeline.html", priority: 3},
    {level: 2, id: "tp-constraints", title: "tP: Constraints", link: "tp-constraints.html", priority: 2},
    {level: 2, id: "tp-teams", title: "tP: Forming Teams", link: "tp-teams.html", priority: 2},
    {level: 2, id: "tp-w2", title: "tP week 2: " + weekly_tp_themes.w2.name, link: "tp-w2.html", priority: 2},
    {level: 2, id: "tp-w3", title: "tP week 3: " + weekly_tp_themes.w3.name, link: "tp-w3.html", priority: 2},
    {level: 2, id: "tp-w4", title: "tP week 4: " + weekly_tp_themes.w4.name, link: "tp-w4.html", priority: 3},
    {level: 2, id: "tp-w5", title: "tP week 5: " + weekly_tp_themes.w5.name, link: "tp-w5.html", priority: 2},
    {level: 2, id: "tp-w6", title: "tP week 6: " + weekly_tp_themes.w6.name, link: "tp-w6.html", priority: 2},
    {level: 2, id: "tp-w7", title: "tP week 7: " + weekly_tp_themes.w7.name, link: "tp-w7.html", priority: 2},
    {level: 2, id: "tp-w8", title: "tP week 8: " + weekly_tp_themes.w8.name, link: "tp-w8.html", priority: 3},
    {level: 2, id: "tp-w9", title: "tP week 9: " + weekly_tp_themes.w9.name, link: "tp-w9.html", priority: 2},
    {level: 2, id: "tp-w10", title: "tP week 10: " + weekly_tp_themes.w10.name, link: "tp-w10.html", priority: 2},
    {level: 2, id: "tp-w11", title: "tP week 11: " + weekly_tp_themes.w11.name, link: "tp-w11.html", priority: 2},
    {level: 2, id: "tp-w12", title: "tP week 12: " + weekly_tp_themes.w12.name, link: "tp-w12.html", priority: 3},
    {level: 2, id: "tp-w13", title: "tP week 13: " + weekly_tp_themes.w13.name, link: "tp-w13.html", priority: 2},
    {level: 2, id: "tp-deliverables", title: "tP: Deliverables", link: "tp-deliverables.html", priority: 2},
    {level: 2, id: "tp-pe", title: "tP: Practical Exam", link: "tp-pe.html", priority: 2},
    {level: 2, id: "tp-grading", title: "tP: Grading", link: "tp-grading.html", priority: 2},
    {level: 2, id: "tp-supervision", title: "tP: Supervision", link: "tp-supervision.html", priority: 2},
  {level: 1, id: "peerEvaluations", title: "Peer Evaluations", link: "peerEvaluations.html", priority: 2},
  {level: 1, id: "tools", title: "Tools", link: "tools.html", priority: 3},
  {level: 1, id: "participation", title: "Participation Marks", link: "participation.html", priority: 2},
  {level: 1, id: "gradeBreakdown", title: "Grade Breakdown", link: "gradeBreakdown.html", priority: 2},
  {level: 0, id: "appendices", title: "Appendices"},
    {level: 2, id: "appendixA-principles", title: "Apdx A: Module Principles", link: "appendixA-principles.html", priority: 4},
    {level: 2, id: "appendixB-policies", title: "Apdx B: Module Policies", link: "appendixB-policies.html", priority: 1},
    {level: 2, id: "appendixC-faq", title: "Apdx C: FAQ", link: "appendixC-faq.html", priority: 1},
    {level: 2, id: "appendixD-help", title: "Apdx D: Getting Help", link: "appendixD-help.html", priority: 2},
    {level: 2, id: "appendixE-gitHub", title: "Apdx E: Using GitHub", link: "appendixE-gitHub.html", priority: 1},
    {level: 2, id: "appendixF-teamworkIssues", title: "Apdx F: Handling Team Issues", link: "appendixF-teamworkIssues.html", priority: 4}
]%}

{% set weekly_admin_topics = {
week1: [
  {topic_id: "tp-teams"},
  {topic_id: "textbooks"},
  {topic_id: "gradeBreakdown"}
  ],
week2: [
  {policy_id: "policy-plagiarism"},
  {policy_id: "policy-reuse"},
  {policy_id: "policy-techHelp"}
  ],
week3: [
  {topic_id: "peerEvaluations"},
  {topic_id: "standardsAndConventions"},
  {topic_id: "tp-supervision"},
  {policy_id: "policy-teamSize"}
  ],
week4: [],
week5: [
  {topic_id: "tp-grading"},
  {policy_id: "policy-workDistribution"}
  ],
week6: [
  {topic_id: "appendixF-teamworkIssues"}
  ],
week7: [],
week8: [],
week9: [],
week10: [],
week11: [],
week12: [],
week13: []
}%}