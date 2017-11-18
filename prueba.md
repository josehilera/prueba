## Rule

 Property     | Type | Description
|--------------|---------|------
| rule_id    | Text |
| name        | Text |
| test_mode    | [TestModeType](#TestModeType) |
| environment | [EnvironmentType](#EnvironmentType) |
| success_criterion | SuccessCriterion |
| authors | [Person[]](#Person) or Text |
| description | Text |
| background | [BgReference] |
| assumptions | [Assumption] |
| test_procedure | TestProcedure |
| outcome | Outcome |

### TestModeType 

Value     | Description
|--------------|---------
| Automatic   | 
| Semi-automatic        | 
| Manual | 

### EnvironmentType 

Value     | Description
|--------------|---------
| MarkupDocument | As HTTP Response in ACT
| DOMStructure | As DOM Tree in ACT
| WebBrowser | As Rendered page in ACT
| WebDriver   | Not exists in ACT
| Template | Not exists in Auto-WCAG but it exists in ACT
| Script | Not exists in Auto-WCAG but it exists in ACT


