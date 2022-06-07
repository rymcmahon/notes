### See what's running on a port

`lsof -wni tcp:<port>`

### Stop what's running on a port. Use PID listed in output from above

`kill -9 <pid>`

### Mount NVM

`source ~/.nvm/nvm.sh`

### Check NVM version

`nvm ls`

### Fetch one remote branch

`git fetch <remote_name> <branch_name>`

### Checkout to last branch

`git checkout -`

### Rebasing Strategy
```
git checkout -b new-feature main
# work on feature
git commit -a -m "Add feature"
git rebase origin/main

# OR
git checkout -b my-feature -t origin/main
git pull --rebase (since -t told it to track main)
```

### Add existing project to Github

1. git init
2. git add .
3. git commit -m 'first commit'
4. copy the remote repo url
5. git remote add origin <remote_repo_url>
6. git push -u origin master

### New Rails project with PostgreSQL and without Minitest

`rails new <app_name> --database=postgresql --skip-test`

### New Rails project with PostgreSQL, skip Minitest, skip webpack

`rails new app_name --database=postgresql --skip-test --skip-webpack-install --skip-javascript`

### Open Bash Profile in Atom

`atom . ~/bash_profile`

### If dev database is set to prod after pulling down prod db

`bin/rails db:environment:set RAILS_ENV=development`

### Bash Movements

iTerm Mac
control + a = move to start of line
control + e = move to end of line
option + back-arrow = move one word back
option + forward-arrow = move one word forward

Windows
option + b = move one word back
option + f = move one word forward

### Run Dotnet Server on a different port

`dotnet run --urls="http://localhost:5001"`

### Restart OmniSharp if VS Code F12 Go To Definition isn't Working

`command + shift + p -> OmniSharp: Restart OmniSharp`

