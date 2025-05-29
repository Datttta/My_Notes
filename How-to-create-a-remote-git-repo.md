= Steps to create a remote git repository =

1. Follow the image bellow, use "git add ." instead, git push you probably not work

![](media/step1_follow_git_hub_commands.png)

2. Now create a ssh key with "ssh-keygen -t ed25519 -f ~/.ssh/id_<NameOfYourKey>" -C "youreamil" 
   
![](media/Step2creatingkey.png)

3. Use the command bellow with the id_ you created
 
![](media/Step3_git.png)

4. Follow the commands bellow:

![](media/Step4_commands.png)


5. Open ~/.ssh/config and follow the pattern of the image bellow, using the key you created:
 

![](media/Step5_config.png)

Now git push should work.
