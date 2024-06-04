
# Vint Offline Portable

This is portable offline version of the TankiX game.
Just unzip with 7zip-zstd and run.

## Sources

1. [Server and Client](https://github.com/Vint-TX/Vint)
2. [.net runtime](https://download.visualstudio.microsoft.com/download/pr/77650902-a341-4f4c-934f-db7056cbfa78/176d961f8bbc798596f8d498ede4cc73/dotnet-runtime-8.0.5-win-x64.zip)
3. [MariaDB](https://archive.mariadb.org/mariadb-11.3.2/winx64-packages/mariadb-11.3.2-winx64.zip)

## How to run Offline

1. Unzip with [7zip-zstd](https://github.com/mcmilk/7-Zip-zstd/releases)
2. Run start_mariaDB.bat
3. Go in the Vint Server folder and run server_run.bat
4. Go in the Vint Client folder and run vint.exe \
4.1 You can drop goldbox only in matchmaking battle with this command in chat !dropBonus gold
5. When finish playing, close the server and client windows and then run remove_mariaDB_service.bat

6. If you want to keep accounts and users, before running remove_mariaDB_service.bat copy the current mariadb-11.3.2-winx64\bin\db folder in mariadb-11.3.2-winx64\bin\old
7.  If your folder is moved or renamed and Mydb service won't start , open edit the my.ini file it the db folder to ist current correct path \
eg: \
    [mysqld] \
    datadir=C:/path to your folder/your folder/mariadb-11.3.2-winx64/bin/db \
    port=3306 \
    [client] \
    port=3306 \
    plugin-dir=C:/path to your folder/your folder/\mariadb-11.3.2-winx64/lib/plugin 

## Multiplayer Online

1. Setup [Hamachi][https://vpn.net/] or any similar software or VPN
2. Run start_mariaDB.bat
3. Go in the Vint Server folder and run server_run.bat
4. Give the IP to the other player/s who only need to put it in \Vint Client\vint_Data\config\clientlocal\startup\public.yml (replace the two http://127.0.0.1:8080 strings with the IP and Port from Hamachi) and only run \Vint Client\vint.exe
