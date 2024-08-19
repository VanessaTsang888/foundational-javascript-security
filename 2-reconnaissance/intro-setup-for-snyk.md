# Intruction and Setup for Snyk

[Snyk](https://snyk.io/) is a fantastic tool to help us identify issues within our dependencies. It dose it automatically as we make updates to our repository. It provides a lot more deails on vulnerable dependencies, than we get with NPM audit and the specific exploit that could occur.

## How it works

If we don't have an account, click the 'Sign up for free' button and then follow the instructions to connect with our repo. Login and will arrive at the Dashboard.

Connect a project to your snyk account by add a repo. Click the 'Add project' btn. Then select on of the x4 options i.e. we can montior it by GitHub. Once arrived in our GitHub we select a repo we want to include and click the 'Add selected repositories' btn.

Once we have added repos to our Dashboard we can either click on Dashboard or go to Projects menu at the top. We see projects with issues. Click on the left dropdown on an issue report and select a file they have the issue with i.e. 'package.json' file - this is where the dependencies are listed. Click on this file to see what are the issues in more detail. On the left menu select the High checkbox to see all the High severity issues. Now we can see where an issue orginated from. For example the 'ajv@6.12.3' originate from the 'react-scripts@1.1.5'. This way we can go through the owner of that repo (Facebook) and let them know there might be an High security issue with one of these packages we are using in our react scripts repo and maybe open a PR. We click to see more details of that issue in how the issue will impact our app in the end. Do this for every issue we have that is High or Medium (can become High can be script injections or denial of service potential issues like that). We need to do this to ensure our app is as safe as possible for our users.

Then we can open a PR to get vulnerability fixed by the vendor. If we click the 'Partially fix this vulnerability' btn then it will open a PR for that particular package and partially fix it for us. Navigate back to Dashboard and we see the PR we just opened for that one where we fixing all the issues so we can fix those issues ourself.

This is what Snyk offers us, a lot more info about any issues we may have with our applications and the dependencies within our app and how to fix them. ## Vanessa's Notes

## Vanessa's Notes

I like this Snyk tool and I will definately try it in the near future.
