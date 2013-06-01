Symbolic link synchronizer
==========================

The purpose of this script is to make a symbolic link representation of one directory's contents in another. This is especially useful when one wishes to synchronize dotfiles between computers with Dropbox. With this script you can easily create symbolic links in a home directory to those files. 

The symbolic links replace all files and directories in the target directory of the same name as the ones in the source file. Directory names can be specified for directories that are to be left alone if they exist and continue the synchronization inside them. This can be useful in case of the `.config` file, where one doesn't necessarily want to synchronize all directories therein.

I have this script covered with a fair amount of tests, nevertheless, I'd rather not piss someone off accidentally. Also, it's easy to make mistakes using faulty arguments to the script. So __make a backup__ of your files if in doubt.

Here's an example usage to synchronize one's dotfiles with the ones saved in a Dropbox directory:
`symsync ~/Dropbox/linuxfiles/dotfiles ~/ .config`


