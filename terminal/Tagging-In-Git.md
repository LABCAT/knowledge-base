This is a basic example of how to do tagging in git. 

## How to Create a New Tag

Fetch all tags:

git fetch --tags

Then check what the latest tag is with the following command:

git tag

Then create a new tag which doesn’t already exist:

git tag -a 1.0.0 -m "creating tag 1.0.0 - 1st January 2020"
git push origin --tags

## How to Delete a Tag

From the remote repository:

git push --delete origin tagname

From your local repository:

git tag --delete tagname

## How to Checkout a Tag

git fetch --tags
git checkout 3.0.0

## How to Tag from a Specific Commit

git tag -a 1.2 56f78f210cca7d181315bc3d1eb2c366045ee86f-m "Creating tag 1.2"
