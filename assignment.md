Your login name: altschool i.e., home directory /home/altschool. The home directory contains the following sub-directories: code, tests, personal, misc Unless otherwise specified, you are running commands from the home directory.

| Task | Task Description                                                                                  | Solution                                                                | Image                                              |
| ---- | ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | -------------------------------------------------- |
| a    | Change to the tests directory using absolute pathname                                             | cd /home/altschool/tests                                                | ![1707563286385](image/assignment/1707563286385.png) |
| b    | Change to the tests directory from your home directory using relative pathname                    | cd ./test                                                               | ![1707564004682](image/assignment/1707564004682.png) |
| c    | Use echo command to create a file named fileA with text content ‘Hello A’ in the misc directory | **echo 'Hello A' > /home/altschool/misc/fileA**                   | ![1707564593485](image/assignment/1707564593485.png) |
| d    | Create an empty file named fileB and populate it with dummy contents                              | echo 'Dummy Content' sudo tee /home/altschool/misc/fileB> /dev/null     | ![1707566083429](image/assignment/1707566083429.png) |
| e    | Copy contents of fileA into fileC                                                                 | sudo cp /home/altschool/misc/fileA /home/altschool/misc/fileC           | ![1707566164453](image/assignment/1707566164453.png) |
| F    | Move contents of fileB into fileD                                                                 | **sudo mv /home/altschool/misc/fileB /home/altschool/misc/fileD** | ![1707566681325](image/assignment/1707566681325.png) |
| G    | Create a tar archive called misc.tar for the contents of misc directory                           | sudo tar cvf /home/altschool/misc.tar -C /home/altschool misc           | ![1707566823428](image/assignment/1707566823428.png) |
| H    | Compress the tar archive to create a misc.tar.gz file                                             | sudo gzip /home/altschool/misc.tar                                      | ![1707567266311](image/assignment/1707567266311.png) |
| I    | Create a user and force the user to change his/her password upon login                            | Lock a users password                                                   | ![1707568342239](image/assignment/1707568342239.png) |
| J    | Lock a users password                                                                             | **sudo passwd -l UserA**                                          | ![1707568543340](image/assignment/1707568543340.png) |
| K    | Create a user with no login shell                                                                 | **sudo useradd -M -s /usr/sbin/nologin UserA**                    | ![1707568801868](image/assignment/1707568801868.png) |

| L | Disable password based authentication for ssh | sudo nano /etc/ssh/sshd_config | ![1707570132759](image/assignment/1707570132759.png) |
| - | --------------------------------------------- | ------------------------------ | -------------------------------------------------- |
| M | Disable root login for ssh                    | sudo nano /etc/ssh/sshd_config | ![1707570142774](image/assignment/1707570142774.png) |
