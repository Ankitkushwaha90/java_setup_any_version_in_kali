# two method for java setup in environment after installation in tar.gz 

# and commands for extract tar.gz file =>sudo tar -xf filename.tar.gz

- 1.check path for commands => $PATH

```bash
export PATH="$PATH:/usr/lib/jvm/jdk-22.0.1/bin"
export PATH="$PATH:/usr/lib/jvm/jdjdkk/bin/java"
                         
export PATH="$PATH:/usr/lib/jvm/jdjdkk/bin/javac"
```

- 2.write can be directe in file => sudo nano /etc/environment

- 3. setup for choise any one version of java
```bash
sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdjdkk/bin/java"
sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdjdkk/bin/javac"
sudo update-alternatives --set java /usr/lib/jvm/jdjdkk/bin/java
sudo update-alternatives --set java /usr/lib/jvm/jdjdkk/bin/javac
```

- 4. final

   ┌──(root㉿kali)-[/usr/lib/jvm/jdk-22.0.1/bin]
└─# sudo update-alternatives --config java

There are 4 choices for the alternative java (providing /usr/bin/java).

  Selection    Path                                         Priority   Status
------------------------------------------------------------
  0            /usr/lib/jvm/java-21-openjdk-amd64/bin/java   2111      auto mode
* 1            /usr/lib/jvm/java-17-openjdk-amd64/bin/java   1711      manual mode
  2            /usr/lib/jvm/java-21-openjdk-amd64/bin/java   2111      manual mode
  3            /usr/lib/jvm/jdk-22.0.1/bin/java              0         manual mode
  4            /usr/lib/jvm/jdk-22.0.1/bin/javac             0         manual mode

Press <enter> to keep the current choice[*], or type selection number: 4
update-alternatives: using /usr/lib/jvm/jdk-22.0.1/bin/javac to provide /usr/bin/java (java) in manual mode
                                                                                                                                                                      
┌──(root㉿kali)-[/usr/lib/jvm/jdk-22.0.1/bin]
└─# 


