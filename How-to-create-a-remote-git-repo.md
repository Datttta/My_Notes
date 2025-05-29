= Steps to create a remote git repository =

1. Follow the image bellow, use "git add ." instead, git push you probably not work

![](../Pictures/screenshots/swappy-20250528-210511.png)
2. Now create a ssh key with "ssh-keygen -t ed25519 -f ~/.ssh/id_<NameOfYourKey>" -C "youreamil" 
   
![](media/Step2creatingkey.png)
3. Use the command bellow with the id_ you created
 
![](../Pictures/screenshots/swappy-20250528-210634.png)
4. Follow the commands bellow:

![](../Pictures/screenshots/swappy-20250528-211028.png)
5. Open ~/.ssh/config and follow the pattern of the image bellow, using the key you created:
 
![](../Pictures/screenshots/swappy-20250528-211048.png)

Now git push should work.
