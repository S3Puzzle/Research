# How can I use a custom git runner to improve my ci/cd pipeline?

## Question exploration

What information is available?
- Literature study

What are the advantages of a custom runner?
- Literature study

How can I implement the available information?
- Brainstorm

How do you make a git runner?
- Prototyping

What is quality of my product?
- System test

## What information is available?

After some online research I found that github has documentation on git runners. On githubs docs there are multiple pages dedicated to git runners. There is a page on the differences between standard runners and self-hosted runners. There is also a page on how to make a self-hosted runner. On youtube I found a lot of additional tutorials on how to make git runners.

## What are the advantages of a custom runner?
One of the most important advantages of using a self-hosted runner is that they are more customizable. An other advantages is that unlike the standard github runner, an self-hosted runner doesn't need to have a clean instance for every job execution. There is also a financial advantage. The github runner is only free for a set amount of minutes per month. Once setup it can be way cheaper to have a self-hosted runner.

https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners

