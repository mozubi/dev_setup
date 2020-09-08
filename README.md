# Setup instructions

The following instructions will setup a local development environment:

## Vagrant

Vagrant is a tool for building and managing virtual machine environments in a single workflow. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases production parity, and makes the "works on my machine" excuse a relic of the past.

[Download vagrant 2.2.9](https://www.vagrantup.com/downloads)

## Oracle VM VirtualBox
VirtualBox will run the actuall virtual machine on your computer. If you want to learn more about VMs: [https://en.wikipedia.org/wiki/Virtual_machine](https://en.wikipedia.org/wiki/Virtual_machine).

[Download Virtualbox - Version 5.2.449](https://www.virtualbox.org/wiki/Download_Old_Builds_5_2)


## Download rails_box from github




4. Activate virtualization in bios(if not working)
5. Terminal - navigate to dev_box, run vagrant up
6. Download vscode
7. Install RemoteSSH Extension
8. Terminal -> vagrant ssh-config -> copy info from terminal
9. click vscode RemoteSSH icon -> left corner
10. click on first list item
11. copy the config info
12. click vscode RemoteSSH icon -> left corner
13. connect to host, retry if fails, select Linux in the new window if given a choice
14. set git credentials locally
15. connect to github
https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account
16. clone mozubi/plattform repo(via ssh or https)
17. open project: Terminal -> code .
18. $ bundle install, $ yarn install
19. $ rbenv rehash
20. login to heroku in your browser, Terminal: $ heroku login -i
21. pull the db data locally: Terminal: $ heroku pg:pull mozzubi::RED mozubi_offcial_development -a mozzubi
22. Start server: $ bin/rails server -b 0.0.0.0
23. check app in browser at: http://localhost:3000/
24. $ bundle exec rake db:create RAILS_ENV=test
25. $ rake db:test:prepare
22. Happy coding
