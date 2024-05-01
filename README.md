# Fix Regex in Logrhythm

* Go in MPE Rule Builder
* clone rule
* Import log message manually
* Test all
* Fix regex in https://regex101.com/
  - Select # instead of / in regular expression
  - then try with Regex Debugger to make your regex works
* Match a new parameter with subrule condition
* Clone subrule, create field Tag2 in your regex for example  'log_subtype="(?<tag2>[^"]+)" ' then trigger on subrule when <tag2> = Denied for example
* Edit sub-rule sorting
* edit rule to test
* then synchronise sub-rule to test with Synchronize with based_rule -> Rule status
* Save rule
* Go to log processing policies
* clone the target policy with type custom
* go to log source -> your source -> select the cloned policy instead of the default
* go to mpe rule builder -> open -> edit -> edit rule base sorting, and put your custom rule at the top 
