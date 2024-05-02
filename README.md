two method for java setup in environment after installation in tar.gz 

and commands for extract tar.gz file =>sudo tar -xf filename.tar.gz

1.check path for commands => $PATH 

                          => export PATH="$PATH:/usr/lib/jvm/jdk/bin"
                          
                          => export PATH="$PATH:/usr/lib/jvm/jdk/bin/java"
                          
                          => export PATH="$PATH:/usr/lib/jvm/jdk/bin/javac"
                          
2.write can be directe in file => sudo nano /etc/environment
