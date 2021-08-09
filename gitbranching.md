**git branching**

We will be using two (2) types of git branch prefixes:

- feature: This prefix will be used when a branch is used to build out a new feature for the produt. For instance when you are working on a ticket for the first time.

- fix or patch: This prefix will be used when you are trying to fix a bug or trying to improve a particular feature on the product. For instance if we find a bug / improve the behaviour in a feature linked to a ticket that has already been merged to production.




**branch naming convention**

For example, a [setup-blah-blah-blah]() ticket. A good naming convention for the branch would be:

- **Pre merge**: `feature/setup-blah-blah-blah`
- **Post merge**: `fix/setup-blah-blah-blah` or `patch/setup-blah-blah-blah`
