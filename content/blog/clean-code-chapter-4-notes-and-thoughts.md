---
title: Clean Code Chapter 4 Comments Notes and Thoughts
description: Notes and thought on the Chapter 4 "Comments" of Robert C. Martin's seminal book "Clean Code".
date: 2023-03-30
draft: true
---

{% include "clean-code-banner.njk" %}

## Chapter Comments
TBD
  

## Chapter Notes
Comments can be helpful, clutter the codebase or be misguiding when not updated. Code is neccessary eveil.

Comments are meant to communicate what we fail to communicate with code. Comments are always failures and should and should it. If possible, is better to communicate the idea using code.

Comments become stale and is not realistic that developers can maintain them. Code mutates over time, leaving comments behind in places where they don't make sense.

Although developers should be dissicplined and keep comments up to date is better to use that time to write code in a way that does not need comments. Code should be the single source of responsability.

The use of comments should be minimized.

### Comments Do Not Make Up for Bad Code

Commnets make up for messy and disorganized code whihc is hard to understand. Instead of spending time writting comments, clean up the code instead.

### Explain Yourself in Code

Explain your intent with code instead of using comments. E.g. encapsulate code in fucntions with a descriptive name.

### Good Comments

Some good usage for comments:

#### Legal Comments

Corporate codign standards require to include comments for legal reaons. For example copyright and authority statements. Tehy should not be contracts or too long, refer to a stastandard license instead.

#### Informative Comments

Commnets can add usuful information about a statement, but is better to encapsulate the code into a variable or function with a meaningful name.

#### Explanation of Intent

Provide explanation about the intent of a desicion.

#### Clarification

Commnets can be used to clarify API of external libraries or code that can't be touched. This is risky becasue the comment can be wrong.

#### Warning of Consequences

Warn otehr developers about certain consequwences like avoiding running a command or using a specific method.

#### TODO Comments

To do notes as `// TODO` comments. This are tasks that should be done in the future and act as reminders. They are not a excuse to introduce bad code.

#### Amplification

Amplify the importance of something that may be overlooked.

#### Javadocs in Public APIs

Document public APIs, although they can be outdated.

### Bad Commnents

Crutches or excuses for bad code.

#### Mumbling

Make sure to write comments that make sense and are valuable. If a comment forces you to look for coed to understand it failed to serve it's purpose.

#### Redundant Comments

Avoid comments that explain the code in a redundant fashion.

#### Misleading Comments

Avoid introducing misinforation by providing comments that are not precise enough.

#### Mandated Comments

Don't anide by riles like every fucntion should be explained by a comment. Tehy clutter up the code. They are usually just redundant.

#### Journal Comments

Don't keep tabs of the chagnes of files as comments. Version control systems takes care of keeping tabs on changes.

#### Noise Commments

Avoid comments thta restate teh obvious and provide no new information. We tend to just ignore them and tend to be outdated.

#### Scary Noise

Avoid documentation comments which are redundant, specilly when copied and pasted.

#### Don't Use a Commnet When You Can Use a Function or a Variable

Refactor code to encapsulate commentable code in fucntions or varibles which are intent-revealing.

#### Position Markers

Postion markers are used to mark s particular positon in the document like banners

E.g, `Actions ////////`

They clutter the codebase , when overused developers stop paying attention.

#### Closing Brace Comments

Closing bfraces comments are used to keep track of the statement the corresponds to a closign stement, specally for nested or long blocks of code. TRy to shorten your functions instead.

#### Attributions and Bylines

Are comments that stea who and when something was added to let know other people with whom they talked to if they have questions. Source control systems keep track of this information.

#### Commented-Out Code

Commented out coed is used as a backup or alterante path to test a specific case. It looks important and decide are afarid to delete it. Commented out code degrades,. clutre code and is confusing. Use a version control system instead. If you see commented out code just delete it.

#### HTML Comments

Commetns using HTML to format documentation is hard to understand and follow. Code should be clear where it is closer to being used.

#### Nonlocal Information

Comments should be relevant to the context they are written at. Avoid sytemwide inforamtion in a local comment. The comment wil remain even if to waht they are referring to change.

#### Too Much Information

AVoid details and historical discussion. 

#### Inobvious Connection

The connection between the comment and the code it describes should be obvious. 

#### Function Header

Prefer short functions instead of fucntion headers.

#### Javadocs in Nonpublic Code

Teh formality of javadocs don't provide any value for local code.