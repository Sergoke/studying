sudo ::: super user do
su ::: super user

apt ::: advanced packaging tool(new from 2014){
    apt install /package name/
    apt update ::: update sources list
    apt upgrade ::: install available upgrades of all packages on system
    apt search /package name/
    apt remove /package name/ remove package without configuration data
    apt purge /package name/ remove package with data in config file
    apt show /package name/ ::: show package info
}
apt-get ::: advanced packaging tool(old)

screen ::: terminal multiplexer{
    screen -S /session name/ ::: create new screen session
    screen -ls ::: list existing screen sessions
    screen -r /pid || session name/ ::: resume  a detached screen session
    screen -X -S /pid || session name/ /command/ ::: send  the  specified command to a running screen session

    ^a + d ::: detach screen from current screen session
    ^a + k ::: kill this window
    ^a + \ ::: kill all windows
    ^a + c ::: create new window
    ^a + w ::: list all windows
    ^a + " ::: list all windows with opportunity to choose
    ^a + n / ^a + p ::: next window / previous window
    ^a + /window number/ ::: switch to window with specific number
}