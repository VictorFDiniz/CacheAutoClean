_Languages:_ <a href="https://github.com/VictorFDiniz/CacheAutoClean/blob/main/README.pt-br.md">Português-br<a/>, <a href="https://github.com/VictorFDiniz/CacheAutoClean/edit/main/README.md">English</a>

![auto](https://user-images.githubusercontent.com/86570043/132133920-1b91914e-0043-4f92-950f-e66faf8482a0.png)

## Install command for CentOS, Debian and Ubuntu
```
wget -c -P $HOME https://raw.githubusercontent.com/VictorFDiniz/CacheAutoClean/main/install.sh; cd $HOME; chmod +x install.sh; ./install.sh
```

## About this script
If you have a server that doesn't have enough RAM, crashes frequently, and you don't have the budget for an upgrade, this script can help you! You can set a limit value for RAM usage. If the value is reached, the script automatically clears the cache allocated in RAM to prevent the server from crashing. It's also possible to configure Swap memory via Swappiness to alleviate RAM usage when it reaches a certain threshold.

There are three cleaning options:
  
![auto02](https://user-images.githubusercontent.com/86570043/132132958-05897109-85ff-4191-9cd1-d4bbf168d426.png)
  
Clearing the cache in production environments may not be a good idea. But if you still decide to use the script in your production environment, the first option (PageCache clearing) is the safest.
  
![auto03](https://user-images.githubusercontent.com/86570043/132133554-a61fd8bc-aac6-4696-a680-daa6dc4c65d5.png)

Or just skip and go straight to the swappiness configuration.

## Commands
```
Usage: cachecln <value> ramtrig <value>
Example: cachecln 2 ramtrig 45

autoclean stop, to stop
autoclean start, to start when stopped
autoclean restart, to restart
autoclean remove, to remove the script
```
