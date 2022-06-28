### WSL
- Enable WSL on Windows in the Command Line<br />
`Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

- Install Ubuntu in Microsoft Store [here](https://apps.microsoft.com/store/detail/ubuntu-1804-on-windows/9N9TNGVNDL3Q)

- Run Ubuntu and run the command to upgrade the repository:<br />
`sudo apt update`

### Fish Shell on WSL

- Install Fish<br />
`sudo apt install fish`

- Run Fish Shell<br />
`fish`

- Install curl<br />
`sudo apt install curl`

- Install powerline fonts<br />
`sudo apt install fonts-powerline`

- Install Oh My Fish<br />
`curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish`

- Set fish as a default shell<br />
`chsh -s /usr/bin/fish`


### NodeJS<br />
- Install NVM</br>
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash`

- Install NVM to update NodeJS for Oh My Fish<br />
`omf install https://github.com/fabioantunes/fish-nvm`<br />
`omf install https://github.com/edc/bass`

- Install latest NodeJS version<br />
`nvm install 16.13.1`

- Switch Node versions:<br />
`nvm use 16.13.1`

### PostgreSQL<br />
- Install PostgreSQL on WSL:<br />
`sudo apt install postgresql postgresql-contrib`

- Confirm installation:<br />
`psql --version`

- Create a postgres user and set the password for the user postgres:<br />
`sudo passwd postgres`

- Start running the database:<br />
`sudo service postgresql start`

- Connect to the postgres service and open the psql shell: <br />
`sudo -u postgres psql`

- Change password in case authentication failed:<br />
`ALTER USER postgres WITH PASSWORD 'password';`

## Git

- Add a PPA (Personal Package Archive), maintained by the Git team for Ubuntu users<br/>
`sudo add-apt-repository ppa:git-core/ppa`

- Update git<br/>
`sudo apt install git`

- Change visudo editor from nano to vim: <br />
`sudo update-alternatives --config editor`

This will show a table like this: 

```
There are 4 choices for the alternative editor (providing /usr/bin/editor).

  Selection    Path                Priority   Status
------------------------------------------------------------
* 0            /bin/nano            40        auto mode
  1            /bin/ed             -100       manual mode
  2            /bin/nano            40        manual mode
  3            /usr/bin/vim.basic   30        manual mode
  4            /usr/bin/vim.tiny    10        manual mode

Press enter to keep the current choice[*], or type selection number: 3
```
Find `vim.basic` or `vim.tiny` and press the selection number and Enter.
