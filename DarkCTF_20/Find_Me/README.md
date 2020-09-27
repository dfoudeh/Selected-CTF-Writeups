# Find me

![1](images/1.png)

If a running program still has a file that has has been deleted open, you can recover the file throught the open file descriptor. This is located in `proc/pid/fd`.

![2](images/2.png)

We see a process called pass running, lets make note of the pid and and look in proc.

![2-2](images/2-2.png)

We found a password. The fact that it is mysecondpassword gives us a hint that it is the password for the second user account.

![3](images/3.png)

Wolf2 has a lot of directories and subdirectories in the home folder. Lets see if we can grep2win.

![4](images/4.png)

Looks like a flag, but its not the correct one. (The spaces might be a hint) But it tells us we are stading in the right place so we are close. 

![5](images/5.png)

Looking at the file nice_work,it is an exectuable, so lets run it.

![6](images/6.png)

There's our flag backwards. 

darkCTF{w0ahh_n1c3_w0rk!!!}