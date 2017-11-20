## Harmonization ACT Auto-WCAG
|ACT | Auto WCAG
|----|---------
|3.3. Accessibility Requirements | success_criterion
|3.4. Limitations, Assumptions or Exceptions|Background, Assumptions
|4. test subject types HTTP Response, DOM Tree, Rendered Page, Template, Script | environment: Markup Document / DOM Structure / Web Browser / WebDriver 
| 5.2. Test Cases: Each rule contains one or more test cases | until now each rule have one test case
| 6. Rule grouping: To ensure rules are kept small and atomic, they SHOULD be put into a rule-group instead | Until now no rule group
|8. MUST have at least the following properties:
test (Rule ID), subject (Web page), pointer (Selected item), outcome (Passed, Failed or Undetermined) | The resulting assertion is as follows: type= Assertion, test=auto-wcag:rule-id, subject=*the selected element*, mode=automatic,  result = <One TestResult from below> outcome=Failed , description , None of the elements referenced by aria-describedby exists
