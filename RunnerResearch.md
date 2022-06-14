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
One of the most important advantages of using a self-hosted runner is that they are more customizable. An other advantages is that unlike the standard github runner, an self-hosted runner doesn't need to have a clean instance for every job execution. There is also a financial advantage. The github runner is only free for a set amount of minutes per month. Once setup it can be way cheaper to have a self-hosted runner. A self-hosted runner can also be a lot faster than the standard git runner. For the standard git runner you have to wait in a queue before your workflow gets executed, while a self-hosted runner can start right away.(https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners)

## How can I implement the available information?
I will select an tutorial to follow. This selecting is based on multiple factors, one of them being how easy they are to implement. After that I will use the tutorial in combination with the information on github docs to make my self-hosted runner.

## How do you make a git runner?
I decided on using this the tutorial, it was very clear and didn't need additional programs. This in combination with the directions github it self provides, when you add a new runner, helped me create my first selfhosted runner. The steps were staight forward and I managed to create a simple windows runner on my desktop. Here you can see where I made the runner. You can also see that the runner is running.

![image](https://user-images.githubusercontent.com/49039524/173041063-5a3abe34-21c7-4203-bb2d-e30b7302792b.png)


https://www.youtube.com/watch?v=SASoUr9X0QA

## What is quality of my runner?
I tested the runner on my project. It didn't work at first, because of the my desktop was set to refuse to run scripts. After changin the execution policy off my localmachine, running scripts was possible. The only remaining problem is that my self-hosted runner runs on windows. This is a problem when I want to use it for my project in this semester. The reason for this is, that I setup a mysql database in my workflow. The setup code is linux and I have not yet figured out how to translate it to windows.

Changing the execution policy: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-7.2

## Conclusion
After making my one self-hosted runner and testing it, I draw the following conclusions. The biggest advantage for simple project like mine is not having to wait in a queue. In my individual project and group project I noticed that the queue can take an minute and if you want to push often, this is costing you a lot of time. The advantage of having not being limited by the git runner time limit is hard to test for me. I can imagine it being a big deal in larger project, but on the scale i am working on it is not going to be an issue. The customizability is something that can be a big help. Not having to start on a clean instance everytime can help with certaint tests.The easiest operating sytem to test with is in my eyes linux. Because I have a window machine, I made a windows runner. If I choose to make a self-hosted for a future project, I would try to make one on a linux machine.
