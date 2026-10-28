# Failure modes of our issue-to-pr workflow

| Failure | How it shows up | Detection | Recovery | Owner |
| --- | --- | --- | --- | --- |
| Agent invents a path | import error in tests | unit tests after each step | revert the step, rerun with the real path | the person who started the run |