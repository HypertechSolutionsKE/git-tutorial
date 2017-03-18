#git Setup
access https://github.com/git 
Register a new account
Go to terminal by pressing Ctr+Alt+T
Enter the following commands
sudopat-get install git-all
After installation is complete, enter the following command on terminal
git config --global user.name "Your name here"
git config --global user.email "Your email here"

#Generating the SSH Key
Generate a ssh Key by writing on terminal the following code:
ssh-keygen -t rsa -C
Then install pb copy by typing the following command on terminal 
sudo apt-get install xclip -y
type the following comand on terminal *(Assuming you have installed Sublime text. Otherwise install Sublime text)
subl ~/.bashrc
source ~/.bashrc
Then copy the following content at the end of the content in .bashrc file and save
"alias pbcopy='xclip -selection clipboard'
alias pbpaste='xclip -selection clipboard -o'"
from there type this command in the terminal
pbcopy < ~/.ssh/id_rsa.pub

Go to the git account online and select setting->SSH and GPG Keys
go to new SSH keys.
Enter a title and press Ctr+V to paste the SSH key  and save.

#How to generate GPG Key
