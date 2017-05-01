# DEMO


### <q> Before getting into next-step learn what is ssh and vagrant </q> 

- [File - An info about SSH ](https://support.suso.com/supki/SSH_Tutorial_for_Linux)

- [Book - An Introduction to Programming in Go](https://www.golang-book.com/books/intro)

- [Docs - About Vagrant ](https://www.vagrantup.com/intro/index.html)


## Steps to make and edit a vagrant file and to use it .

> 1. Create a new directory and make gitclone into to :

``` 
cb@cb-HP-15-Notebook-PC:~$ mkdir svec
cb@cb-HP-15-Notebook-PC:~$ cd svec
cb@cb-HP-15-Notebook-PC:~/svec$ git clone https://github.com/siva5963/svec_demo.git
Cloning into 'svec_demo'...
remote: Counting objects: 42, done.
remote: Compressing objects: 100% (32/32), done.
remote: Total 42 (delta 5), reused 42 (delta 5), pack-reused 0
Unpacking objects: 100% (42/42), done.
Checking connectivity... done.
cb@cb-HP-15-Notebook-PC:~/svec$ 
```

> 2. Entering into the clonned file and making vagrant to run 

```
cb@cb-HP-15-Notebook-PC:~/svec$ ls
svec_demo
cb@cb-HP-15-Notebook-PC:~/svec$ cd svec_demo
cb@cb-HP-15-Notebook-PC:~/svec/svec_demo$ ls
java  README.md  vagrantfile
cb@cb-HP-15-Notebook-PC:~/svec/svec_demo$ vagrant status
Current machine states:

demo-node                 not created (virtualbox)

cb@cb-HP-15-Notebook-PC:~/svec/svec_demo$ vagrant up 
```
> 3. Checking the vagrant status and you can SSH into the machine :

``` 
cb@cb-HP-15-Notebook-PC:~/svec/svec_demo$ vagrant status
Current machine states:

      go-node                   running (virtualbox)
      
cb@cb-HP-15-Notebook-PC:~/svec/svec_demo$ vagrant ssh go-node 
Welcome to Ubuntu 16.04.2 LTS (GNU/Linux 4.4.0-75-generic x86_64)

       * Documentation:  https://help.ubuntu.com
       * Management:     https://landscape.canonical.com
       * Support:        https://ubuntu.com/advantage

        8 packages can be updated.
      0 updates are security updates.


        Last login: Mon May  1 04:34:37 2017 from 10.0.2.2
vagrant@go-node:~$ 
```
        
```
vagrant@go-node:~$ ls
  go
vagrant@go-node:~$ cd go
vagrant@go-node:~/go$ ls
  bin
  ```
  <hr> now you can write and run go language using VIM using .go files...</hr>
  
  
 
      
      

