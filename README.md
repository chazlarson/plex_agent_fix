# plex_agent_fix

# Linux Install

Clone Repo

`wget https://packages.microsoft.com/config/ubuntu/16.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb`

`sudo dpkg -i packages-microsoft-prod.deb`

`sudo apt-get update`

`sudo apt-get install apt-transport-https`

`sudo apt-get update`

`sudo apt-get install dotnet-runtime-3.1`

`sudo apt-get install -qqy sqlite3 libsqlite3-dev`

# Configuration File

fill out config.json
required fields are:

plexUser
plexPass
plexProtocol
plexPort
plexHost
sectionsToProcess


# Agent Fix
`dotnet ./MonkFixPlexDB.dll --agentfix --verbose`

# Remove Unavailable Files
`dotnet ./MonkFixPlexDB.dll --remove --verbose`
