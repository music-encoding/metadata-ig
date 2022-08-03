# metadata-ig
The repository of the Metadata Interest Group

## What is it for?
This is a workspace for the metadata IG to store (code) snippets, examples and blocks of text for further development. This is also a place for managing discussions and issues that the IG cares about.

## Who manages this?
The IG understands itsself as selfmanaged. The administrative co-chairs have admin access to this repo, but everybody who is an active member of the ig can ask for basic managing rights.

For the metadata IG an active member is somebody who regularly attents the IG meetings.

(Of course, the technical team of the MEI community also has admin access.)

## The structure
There is no defined structure for this repository at the moment.
It is recommended to organize the folders thematically.

## How to contribute to the IG
### Workflow (discussions, issues)

Contribution is always welcome! There are several ways for it:

- Diskussions: This should be some kind of 'save place' for everyone (newbies, old hands, etc.) to come up with everything that is on their mind: questions, ideas (that can be very vage), announcements, polls, etc. All you have to do ist to [open a discussion](https://github.com/music-encoding/metadata-ig/discussions) and you'll get feedback from the community. Every time you open a discussion please choose a category to make them easier to manage.
- Issues: If there is something the IG should work on or something that should be discussed in an IG-meeting (e.g., improvement proposals to the schema) just [open an issue](https://github.com/music-encoding/metadata-ig/issues).Every time you open an issue please label them for easier management. In comparison to a discussion an issue is something that needs work and is understand as a todo for the IG.
- Pull Requests: If you like to contribute to this repository by adding some code please [open a pull request](https://github.com/music-encoding/metadata-ig/pulls).

### Gitflow (IG repository)
- Pushing directly to the directory is not recommented. Please use always the [pull request](https://github.com/music-encoding/metadata-ig/pulls) feature. This makes it easier to manage the code and improves the documentation. (E.g., if release notes are generated automatically they will only document the accepted.)

### Contributing to music-encoding as metadata IG
The workflow to contribute to the schema and guidelines is different to the workflow described above. (see also [https://github.com/orgs/music-encoding/projects/2#card-83741232](https://github.com/orgs/music-encoding/projects/2#card-83741232))

- If you haven't done already please fork the [music-encoding](https://github.com/music-encoding/music-encoding) repository (with your private account) 
- Open a new branch (at your fork) for working. Do not use the develop branch! This will complicate updates from the main repo (upstream pulls).
- When someone pushes code on behalf of someone else it is required to clarify this in a comment to the commit message (see [multi author commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors)). That means: Enter new line after the commit message (new line for each author). If the content is the result of a discussion in the IG the first Co-autor is `@music-encoding/ig-metadata`. All other co-authors will be named afterwads, each in a new line:
    - Co-authored-by: @music-encoding/ig-metadata
    - Co-authored-by: @username1
    - Co-authored-by: @username2

Reasons: Git documents the creator of a commit regardless of the content's author. Further, the creator will appear in the contributer statistics of github. By adding co-authors in the way shown above this situation can be counteracted.
 
- If you like to push your code to the community (for review), you have to open a [pull request](https://github.com/music-encoding/music-encoding/pulls) in your private fork to the `ig-metadata` branch in the music-encoding repo (see figure below). This will start the process of contributing.

![Opening pull request to ig-metadata](img/openPR2music-encoding.png)

- If code is to be played back on behalf of the IG, an active member previously determined by the IG opens a pull request from `music-encoding/ig-metadata` to `music-encoding/music-encoding`.