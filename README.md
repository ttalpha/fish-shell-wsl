### WSL
- Install Ubuntu in Microsoft Store

- Run Ubuntu and run the command to upgrade the repository:
`sudo apt update`

### Fish Shell on WSL

- Install Fish
`sudo apt install fish`

- Run Fish Shell
`fish`

- Install curl
`sudo apt install curl`

- Install git
`sudo apt install git`

- Install powerline fonts
`sudo apt install fonts-powerline`

- Install Oh My Fish
`curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish`

- Set fish as a default shell
`chsh -s /usr/bin/fish`


### NodeJS

- Install NVM to update NodeJS
`omf install https://github.com/fabioantunes/fish-nvm
omf install https://github.com/edc/bass`

- Install latest NodeJS version
`nvm install 16.13.1`

### PostgreSQL
- Install PostgreSQL on WSL:
`sudo apt install postgresql postgresql-contrib`

- Confirm installation:
`psql --version`


- Create a postgres user and set the password for the user postgres:
`sudo passwd postgres`

- Start running the database:
`sudo service postgresql start`

- Connect to the postgres service and open the psql shell: 
`sudo -u postgres psql`

- Change password in case of authentication failed:
`ALTER USER postgres WITH PASSWORD 'password';`
