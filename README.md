# SVEC
> first go programing running

# folder creation
>mkdir foldername
  
      sivananda@sivananda-Lenovo-G50-80:~$ mkdir svdc
# change directory
>cd foldername
   
      sivananda@sivananda-Lenovo-G50-80:~$ cd  svdc
  # git clone
    >go to git hub profile and select clone or download copy the link
    
         sivananda@sivananda-Lenovo-G50-80:~/svdc$ git clone https://github.com/siva5963/svec_demo.git
          Cloning into 'svec_demo'...
         remote: Counting objects: 39, done.
            remote: Compressing objects: 100% (34/34), done.
          remote: Total 39 (delta 5), reused 0 (delta 0), pack-reused 0
        Unpacking objects: 100% (39/39), done.
       
   >next you type 'ls' command
   
       sivananda@sivananda-Lenovo-G50-80:~/svdc$ ls
        svec_demo
    
    >change directory svec_demo
    
        sivananda@sivananda-Lenovo-G50-80:~/svdc$ cd svec_demo/
    
    >check the vagrant status
    
        sivananda@sivananda-Lenovo-G50-80:~/svdc/svec_demo$ vagrant status
        Current machine states:

        demo-node                 not created (virtualbox)

        The environment has not yet been created. Run `vagrant up` to
        create the environment. If a machine is not created, only the
        default provider will be shown. So if a provider is not listed,
        then the machine is not created for that environment.
    > next you type vagrant up
    
        sivananda@sivananda-Lenovo-G50-80:~/svec/svec_demo$ vagrant up
        Bringing machine 'go-node' up with 'virtualbox' provider...
        ==> go-node: Checking if box 'bento/ubuntu-16.04' is up to date...
        ==> go-node: Configuring cache buckets...
        ==> go-node: Machine already provisioned. Run `vagrant provision` or use the `--provision`
        ==> go-node: flag to force provisioning. Provisioners marked to run always will still run.
        
     >check the vagrant status
         
         sivananda@sivananda-Lenovo-G50-80:~/svec/svec_demo$ vagrant status
          Current machine states:

          go-node                   running (virtualbox)

          The VM is running. To stop this VM, you can run `vagrant halt` to
         shut it down forcefully, or you can run `vagrant suspend` to simply
          suspend the virtual machine. In either case, to restart it again,
          simply run `vagrant up`.
          
          
      >next go to ssh node
      
          sivananda@sivananda-Lenovo-G50-80:~/svec/svec_demo$ vagrant ssh go-node
          Welcome to Ubuntu 16.04.2 LTS (GNU/Linux 4.4.0-75-generic x86_64)

           * Documentation:  https://help.ubuntu.com
           * Management:     https://landscape.canonical.com
           * Support:        https://ubuntu.com/advantage

            8 packages can be updated.
          0 updates are security updates.


            Last login: Mon May  1 04:34:37 2017 from 10.0.2.2
            
      >follow the given steps
      
           vagrant@go-node:~$ ls
            go
          vagrant@go-node:~$ cd go
          vagrant@go-node:~/go$ ls
          bin  

          vagrant@go-node:~/go$ vim hello.go
       type the  below code
       
           package main
            import "fmt"
            func main(){
            fmt.Println("HELLO")
            }
            
         then save and exit you type
         
             :wq
             vagrant@go-node:~/go$ go run hello.go
              HELLO
              
              
         it will show the output

      
     

          
          
      
            

        

