# -----------------------------------------------------
# Adge Denkers
# adge.denkers@gmail.com
# file name: .bash_profile
# date: 2017-08-08
# updated: 2018-01-15
# -----------------------------------------------------
# Adge's Personal Bash Profile
# -----------------------------------------------------
# v. 1.1
# -----------------------------------------------------

# -----------------------------------------------------
# Adge's User Accounts
# -----------------------------------------------------

# ----- Adge's GitHub Account
GITHUBUSER="adgedenkers"

# ----- Adge's GitLab Account
# GitLab Username
GITLABUSER="adge@vaftl.us"

# GitLab Password
GITLABPASS="Sh4pley607*"

# ----- Adge's AWS Keys
# This is published by a secret script that houses the two AWS keys. 

# -----------------------------------------------------



# -----------------------------------------------------
# System Configuration Settings
# -----------------------------------------------------
# ----- Set Default Editor to 'Nano'
export EDITOR=/usr/bin/nano

# ----- Add color to the Terminal
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad

# ----- NVM Directory
export NVM_DIR="$HOME/.nvm"
  . "/usr/local/opt/nvm/nvm.sh"
# -----------------------------------------------------



# -----------------------------------------------------
# Directories and Aliases
# -----------------------------------------------------
# My Private Directory
p="$HOME/.ahd"
alias :p="cd $p"

# My Private Directory
p="$HOME/.ahd"
alias :private="cd $p"

# Keys Directory
keys="$HOME/_keys"
alias :keys="cd $keys"

# Personal Bin Directory
bin="$HOME/bin"
alias :bin="cd $bin"

# System Bin Directory
sysbin="/usr/local/bin"
alias :sysbin="cd $sysbin"

# Personal Dev Directory
dev="$HOME/dev"
alias :dev="cd $dev"

# Amazon Drive
adrive="/Users/adge/Amazon_Drive/Amazon\ Drive"
alias :adrive="cd $adrive"

# Speed Test
alias :speed='speedtest'

# Internet Speed Log
speed_log="/var/log/speed.log"
alias :speed-log="tail -f $speed_log"

# Modify default `ls` command
alias ls="ls -lasG"

# Arduino Libraries
arduino_lib="/Applications/Arduino.app/Contents/Java/libraries"
alias :arduino-lib="cd $arduino_lib"

# Bash Profile
profile="$HOME/.bash_profile"
alias :profile="code $profile"

# Editable Profile
editableprofile="$HOME/bin/afd/my_profile.sh"
alias :editableprofile="code $editableprofile"

# -----------------------------------------------------



# -----------------------------------------------------
# FTL Specific Directories and Aliases
# -----------------------------------------------------

# FTL Folder
ftl="$adrive/FTL"
alias :ftl="cd $ftl"

# FTL Team Repository (Local)
team="$adrive/FTL-Team"
alias :team="cd $team"

# -----------------------------------------------------



# -----------------------------------------------------
# Additional Source Code
# -----------------------------------------------------

# afd+Functions
afdFunctions="$HOME/bin/afd/functions/all-functions.sh"
alias :afdFunctions="code $afdFunctions"
source $afdFunctions

# Server Connection Shortcuts
servers="$HOME/bin/afd/settings/server-logins.sh"
alias :servers="code $servers"
source $servers

# -----------------------------------------------------



# -----------------------------------------------------
# Bash Profile Management
# -----------------------------------------------------

# Edit Bash Profile
alias :be="code $profile"

# Reload Bash Profile
alias :br=". ~/.bash_profile"

# These functions need to be replaced so they make changes
# and then sync these changes up to github, for proper versioning.

# -----------------------------------------------------



# -----------------------------------------------------
# AWS-CLI Configuration Settings
# -----------------------------------------------------

# To install the AWS-CLI on a Mac
alias :install_aws_cli=". /Users/adge/bin/fz/scripts/install_aws_cli_mac.sh"

# Enable the auto-completion capability
complete -C aws_completer aws

# -----------------------------------------------------



# -----------------------------------------------------
# Git Shortcut Functions
# -----------------------------------------------------

:git-update() {
    git add .
    git commit "$@"
    git push
}

:git-save() {
    git add .
    git commit "$@"
    git push
}

# -----------------------------------------------------



# -----------------------------------------------------
# Path Management Functions
# -----------------------------------------------------

function path-add() {
    PATH=$PATH:$1
}

#     Example: 
#        $ path-add /some/folder/name

function path-reset() {
    PATH=""
    PATH=/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
}

# -----------------------------------------------------



# -----------------------------------------------------
# Adge's Personal Functions and Settings
# -----------------------------------------------------


# Create shortcut to get the WAN IP Address
alias :wanip="dig +short myip.opendns.com @resolver1.opendns.com"

# ----- WAN IP Address Logger
function wanip_log() {
    wanip_val=$(dig +short myip.opendns.com @resolver1.opendns.com)
    curr_ts=$(date +"%Y-%m-%d %H:%M:%S")
    echo [$curr_ts] $wanip_val >> /var/log/wan_ip.log

    # previous wan ip is stored in an Env. Variable

    # compare the stored wan ip with the wan ip just received

    # if the two are different, update the Env. Variable, and then somehow notify Adge that a change has taken place - because the AWS security groups with my ip will need to be modified to reflect the new ip
}

# -----------------------------------------------------



# -----------------------------------------------------
# Minecraft Commands
# -----------------------------------------------------

# ----- Start Minecraft Server
alias :mine-server="java -Xmx1024M -Xms1024M -jar /usr/local/bin/mcserver.jar nogui"
alias :minecraft="java -Xmx1024M -Xms1024M -jar /usr/local/bin/mcserver.jar nogui"

# Minecraft Mod Application Directory
mods="$HOME/Library/Application\ Support/minecraft"
alias :mods="cd $mods"

# Minecraft Mod Library (were I keep copies of all my mods)
modlib="$dev/minecraft-mods"
alias :modlib="cd $modlib"

# -----------------------------------------------------
