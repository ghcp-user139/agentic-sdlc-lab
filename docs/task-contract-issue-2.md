#Taskcontract:issue2,deliveredorderscanbecancelled
**Goal:**Deliveredordersmustnotbecancellable(issue#2).
**Context:**AGENTS.md(orderstatemachine),tests/unit/test_orders.py
**Inscope:**app/modules/orders/service.py,tests/unit/test_orders.py,tests/integration/test_orders.py
**Outofscope:**alembic/,.github/,pyproject.toml,anynewdependency
**Acceptance:**-anewunittestfailsonthecurrentcodeandpassesafterthefix-POST/orders/{id}/cancelonadeliveredorderreturns400-`python-mpytesttests/unit-q`passes
**Stopandaskahumanif:**thefixneedsaschemachangeorachangeinthepaymentmodule
**Reviewer:**yoursecondaccount
