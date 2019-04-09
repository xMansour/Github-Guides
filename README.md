# Github Guides  

## Understanding the GitHub flow
GitHub Flow is a lightweight, branch-based workflow that supports teams and projects where deployments are made regularly.  

**Create a branch**  
When you're working on a project, you're going to have a bunch of different features or ideas in progress at any given time – some of which are ready to go, and others which are not. Branching exists to help you manage this workflow.  

When you create a branch in your project, you're creating an environment where you can try out new ideas. Changes you make on a branch don't affect the `master` branch, so you're free to experiment and commit changes, safe in the knowledge that your branch won't be merged until it's ready to be reviewed by someone you're collaborating with.  

>Anything in the `master` branch is always deployable.  

**Add commits**  
This process of adding commits keeps track of your progress as you work on a feature branch.  

Commits also create a transparent history of your work that others can follow to understand what you've done and why. Each commit has an associated commit message, which is a description explaining why a particular change was made. Furthermore, each commit is considered a separate unit of change. This lets you roll back changes if a bug is found, or if you decide to head in a different direction.  

**Open a Pull Request**  
Pull Requests initiate discussion about your commits. Because they're tightly integrated with the underlying Git repository, anyone can see exactly what changes would be merged if they accept your request.  

If you're using a Fork & Pull Model, Pull Requests provide a way to notify project maintainers about the changes you'd like them to consider.  

**Discuss and review your code**  
Once a Pull Request has been opened, the person or team reviewing your changes may have questions or comments. Pull Requests are designed to encourage and capture this type of conversation.  

Pull Request comments are written in Markdown, so you can embed images and emoji, use pre-formatted text blocks, and other lightweight formatting.  

**Deploy**  
With GitHub, you can deploy from a branch for final testing in production before merging to `master`.  

Once your pull request has been reviewed and the branch passes your tests, you can deploy your changes to verify them in production. If your branch causes issues, you can roll it back by deploying the existing `master` into production.  

**Merge**  
Now that your changes have been verified in production, it is time to merge your code into the `master` branch.  


## Hello World
**Create a Branch**  
Branching is the way to work on different versions of a repository at one time.  By default your repository has one branch named `master` which is considered to be the definitive branch. We use branches to experiment and make edits before committing them to `master`.  

When you create a branch off the `master` branch, you’re making a copy, or snapshot, of `master` as it was at that point in time. If someone else made changes to the `master` branch while you were working on your branch, you could pull in those updates.  

Use branches for keeping bug fixes and feature work separate from our `master` (production) branch. When a change is ready, they merge their branch into `master`.  

**To create a new branch**  
1. Go to the repositiory.  
2. Click on the drop down at the top of the file list that syas **branch: master**.  
3. Type a branch name.  
4. Select the blue **Create branch** box.  

**Open a Pull Request**  
Pull Requests are the heart of collaboration on GitHub. When you open a pull request, you’re proposing your changes and requesting that someone review and pull in your contribution and merge them into their branch.  

1. Click the **Pull Request** tab, then click the **New pull request**  
2. In the **Example Comparisions** box, select the branch you made to compare it with the `master` branch.  
3. When you’re satisfied that these are the changes you want to submit, click the big green **Create Pull Request** button.  
4. Give your pull request a title and write a brief description of your changes.  

**Merge your Pull Request**  
1. Click the green **Merge pull request** button to merge the changes into `master`.  
2. Click **Confirm merge**.  
Go ahead and delete the branch, since its changes have been incorporated, with the **Delete branch** button in the purple box.  

