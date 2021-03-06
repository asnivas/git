# Git Forks

> We might be seeing lots of repositories on github from other users. Most of the users will secure their repositories. 
> In that case we can't add or modify code in their repositories. In such cases we need to fork their repositories and
> can make changes. On forking someone's repositories we will have a copy of their repositories into our account.

***How to Fork?***

We need to login to the GitHub WebUI and go to a specific repository of a person that you want. In the right most area
you can a Fork button. On clicking on that button you can get a copy of that repository into your account.

After forking that repository you can clone that repository locally from
your account and you can modify those codes as you need.

> Ex : We have 2 users namely USER1 and USER2. User2 want some code from 
> User1's repository. First User2 need to go to the WebUI and after to the
> repository needed. 

	https://github.com/user1/repository

Click on the fork button. Once the fork completes then he can have that
repository in his account.

	https://github.com/user2/repository

Now he can clone to his local system.

	# git clone https://github.com/user2/repository.git

Here we need to know one thing that user2 can even clone user1's reposi-
tory but he can't push the changes until he is permitted to do so.
