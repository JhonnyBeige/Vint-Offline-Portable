
# Vint Offline Portable

This is portable offline version of the TankiX game.
Just unzip and run.

## Sources

1. [Server and Client](https://github.com/Vint-TX/Vint)
2. [.net runtime](https://download.visualstudio.microsoft.com/download/pr/77650902-a341-4f4c-934f-db7056cbfa78/176d961f8bbc798596f8d498ede4cc73/dotnet-runtime-8.0.5-win-x64.zip)
3. [MariaDB](https://archive.mariadb.org/mariadb-11.3.2/winx64-packages/mariadb-11.3.2-winx64.zip)

## How to run Offline

1. Unzip in any folder
2. Run Master.bat

## Multiplayer Online

1. Setup [Hamachi](https://vpn.net/), [Radmin](https://www.radmin-vpn.com/) or any similar software or VPN
2. Give the IP to the other player/s who only need to put it in \client\vint_Data\config\clientlocal\startup\public.yml (replace the two http://127.0.0.1:8080 strings with the IP and Port from Hamachi) and only run \client\vint.exe
