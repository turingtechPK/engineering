Starting the task
Determine the type of the task given.
Determine to which app does it belong ( admin, user, partner)
Determine whether it should be a component, collection or a page.
Pages
Add comments about the page’s purpose
Structure
Define pages with files and folders.
index.js file root page.
Pages having same parent name or are subpages must be kept in the same folder e.g 
/			will call the root page.
/contact		will call the contact page
/my-site		will call the my-site page
/my-site/about		will call about page of my-site

├── pages
|  ├── index.js
|  ├── contact.js
|  └── my-site
|     ├── about.js
|     └── index.js

This hierarchy must be followed. 
 
Components
Describe the functionality they represent.
Avoid jargon so different disciplines understand its function e.g use authorize instead of sanction or schedule instead of program
Be written in singular, not plural, format.
Add comments about the component’s purpose.
Shared Components
All the base components must be listed in the src folder of shared-components folder e.g ant design components.
It must contain an index file which exports all of the components added into this folder.
The component(file) name should be similar to the folder name.
It must contain an element(related to the component) file.
It must contain an index file that exports this component.

Application Specific
All application specific components must be listed under the collections folder of the respective application.
It must contain an index file which exports all of the components added into this folder.
The component name should be similar to the folder name.
It can contain an element(related to the component) file.
It must contain an index file that exports this component.


Implementing a feature
Following steps must be followed when you start implementing a feature.
Make sure you are on the main branch i.e develop. 
Pull latest changes to this branch.
git pull origin develop
Run yarn install command to install the latest packaged added.
Create a new branch.
git branch your-name/feature-name
Checkout to the new branch.
git checkout your-name/feature-name
Add your work.
Commit your work.
Each commit should contain files that are inter-related.
Add commit messages according to the commit rules defined.
Checkout to develop.
Pull the latest changes in develop.
Run yarn install again to make sure all new packages are installed in your repo.
Checkout to your branch and run:
git rebase develop.
If executing the rebase command runs into conflicts, resolve the merge conflicts first and then push your changes.
Else you can push your branch with command:
git push origin your-name/feature-name
Build your code using yarn build. Fix build errors, push your code.
Create a merge request after pushing the branch by going to Gitlab.
If you have created and pushed a new branch simply visit gitlab you will get this and search for your branch.
Else you can go to the merge request and create a new merge request from there.
Select your source branch that you want to merge and the target branch should be develop.

Committing your work

Always pull the latest changes in the main/master/develop branch before creating a branch.
Create a branch with the following convention: your-name/feature-name. If you are the only one working on this feature. Otherwise, team/feature-name
Avoid spelling mistakes while naming a branch.
Give your feature an appropriate name.
Make sure you have branched from the correct branch.
Add all files into one commit that have inter-related changes.
Add a descriptive message for the commit.


Commit Messages
	Syntax
	Valid commit messages have the structure:

	[type]([scope]):: #[issue-number]{.issue-part} [title] 	// This is the commit title
             		// This blank line separates the commit title from the commit body
[body] 		// This is the commit body. It CAN have multiple lines

[variable] are required variables that must be replaced in a final commit message ([] symbols must be removed)
{variable} are optional variables that must be replaced or removed in a final commit message ({} symbols must be removed)
// Comment are comments that must be removed in a final commit message

Rules
The following rules must be met for a commit message to be valid, the product rule only required for the integrates repository:
[type] variable has to be one of the following:
	rever	// Revert to a previous commit in history
feat   	// New feature
perf	// Improves performance
fix	// Bug fix
refac	// Neither fixes a bug or adds a feature
test	// Adding missing tests or correcting existing tests
style	// Do not affect the meaning of the code (formatting, etc)
sol	// Hacking solution only for writeups and training repo

[scope] variable has to be one of the following:
	front	// Front-End change
back	// Back-End change
infra	// Infrastructure change
conf	// Configuration files change
build	// Build system, CI, compilers, etc (scons, webpack...)
job	// asynchronous or scheduled tasks (backups, maintenance...)
cross  // Mix of two or more scopes
doc	// Documentation only changes
A Commit title must exist.
A Commit title must not contain the ':' character.
Commit title must have 60 characters or less.
Commit title must be lower case.
Commit title must not finish with a dot '.'.
Commit title must reference an issue.
Commit title must be meaningful. Avoid using things like feat(build)[integrates]: #5.1 feature.
If commit title has sol type, it must reference issue #0.
A blank line between commit title and commit body must exist.
A commit body must exist.
Lines in commit body must have 72 characters or less.


Example
Here is an example of a compliant commit message (Notice how the issue has a '.1' right after, meaning that such commit is the part 1 for solving the issue):
feat(build): #13.1 add type_check to dangerfile
- Add type_check function to dangerfile
- Remove unnecessary print_output function from dangerfile
Merge Request Messages

Differences with commit messages
Merge Request commits are like commit messages with only two differences:
Merge Request [type] has to be the most relevant type of all its commits. The relevance list is:
rever
feat
perf
fix
refac
test
style
sol

Where revert has the highest and sol the lowest relevance.
For example, if your MR has one feat, one test and one style commit, the [type] of your MR must be feat.
They can (not mandatory) implement a Closes #{issue-number} in their footer, which triggers the automatic closing of the referenced issue once the MR gets accepted
	

Example
Here is an example of a compliant Merge Request Message:
feat(build): #13.3 new checks to dangerfile

- Add type_check
- Add deltas_check
- Add commit_number check

Closes #13
Issue number 13 will be automatically closed once this MR is accepted due to the Closes #13 footer.
