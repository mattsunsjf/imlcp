# iMLCP (Interactive MLCP Shell)

iMLCP is an interactive shell for MarkLogic Content Pump.

Author: mattsun

## Dependency

* [jlineEnhanced](https://github.com/mattsunsjf/JlineEnhanced) A friendly fork of jline2 with specific enhancement for iMLCP 
* [MLCP](http://developer.marklogic.com/products/mlcp) MarkLogic Content Pump, an open-source, Java-based command-line tool that provides the fastest way to import, export, and copy data to or from MarkLogic databases 

## Features

* Run any command of MLCP. Use iMLCP same way as mlcp.sh if you are already familiar with it
* Interactive (Read-Eval-Print Loop)...
* Auto-completion: MLCP command, options, frequently-used value (true, false, xml, ...) and system path
* Command history (hit up arrow)
* Run any system shell command
* Easy to deploy
* Get rid of many existing system shell limitations, include but not limit to:
  * No automatic path expanding limitation of system shell (which may cause 'Argument too long' error)
  * No need to use double quote to enclose some fields (Eg. -delimiter "|", since vertical bar has special meaning in system shell)
  * A easy replacement of options_file in some cases (Eg. use tab as delimiter and contains space in csv header)

## Command Documentation

| Command      | Usage                                                  |
| -------------| ------------------------------------------------------ |
| cls/clear    |Clean the screen                                        |
| quit/exit    | Exit the MLCP interactive shell                        |
| $[command]   | Execute system shell command. Example: $ls -al         |
| help         |Help for MLCP                                           |
| CTRL+C       |Stop the MLCP job or discard current command line input |
| ?            |Help for interactive shell                              |

All the commands are case-insensitive (except system shell commands).
