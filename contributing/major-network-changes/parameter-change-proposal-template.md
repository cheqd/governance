# Parameter Change Proposal

**ParameterChangeProposal** defines a proposal to change one or more network parameters. If accepted, the requested parameter change is updated automatically by the proposal handler upon conclusion of the voting period.

## Proposal template

```jsonc
{
  "title": "Insert the title of the Parameter Change Proposal",
  "description": "Insert long description and link to discussion forum",
  "changes": [
    {
      "subspace": "gov",
      "key": "votingparams", // this is the name of the parameter being changed 
      "value": {"votingperiod":"432000"} // this is the NEW parameter value 
    }
  ],
  "deposit": "8000000000000" //ncheq
}
```
