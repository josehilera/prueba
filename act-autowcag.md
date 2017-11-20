## Comparison of ACT and Auto-WCAG
|ACT | Auto WCAG
|----|---------
|Section 3.1: "Each ACT Rule MUST provide descriptive title" | OK, field "name". 
|Section 3.1: "Each ACT Rule MUST provide unique identifier" | OK, field "rule_id".
|Section 3.2: "Each ACT Rule MUST have a description" | OK, field "Description". 
|Section 3.3: "Each ACT Rule MUST identify the accessibility requirements to which the rule maps, for example, WCAG 2.0 success criterion" | OK, field "success_criterion". 
|Section 3.4: "Each ACT Rule MUST provide a list of limitations" | REVIEW, because no specific field exists for it. It exists the field "Background", confirm if it is to describe limitations.
|Section 3.4: "Each ACT Rule MUST provide a list of assumptions" | OK, field "Assumptions"
|Section 3.4: "Each ACT Rule MUST provide a list of exceptions" | REVIEW, because no specific field exists for it. It exists the field "Background", confirm if it is suitable to describe limitations.
|Section 4: "The following test subject types are common in accessibility testing: HTTP Response, DOM Tree, Rendered Page, Template, Script" | REVIEW the accepted values for the field "environment", because the names are not the same as ACT, and they do not include types as Template or Script. The allowed values are: Markup Document / DOM Structure / Web Browser / WebDriver 
|Section 4: "Other types of test subjects may be possible. In those cases the ACT Rule MUST include a detailed description of the test subject type" | REVIEW, because the "WebDriver" type is not include in ACT list, and must be described.
|Section 5.1: Test procedure include a "Selector" | OK, field "selector".
|Section 5.2: "Each rule contains one or more test cases" | REVIEW, because until now, Auto-WCAG rules have only one test case.
|Section 5.2: Each test case MUST provide mode (whether test case steps are automated, semi-automated or require manual testing), steps, result, description of the error causing any failing result | REVIEW, because now the mode is assigned to the complete rule, but not to each test case.
| 6. Rule grouping: To ensure rules are kept small and atomic, they SHOULD be put into a rule-group instead | Until now no rule group
|8. MUST have at least the following properties:
test (Rule ID), subject (Web page), pointer (Selected item), outcome (Passed, Failed or Undetermined) | The resulting assertion is as follows: type= Assertion, test=auto-wcag:rule-id, subject=*the selected element*, mode=automatic,  result = <One TestResult from below> outcome=Failed , description , None of the elements referenced by aria-describedby exists
