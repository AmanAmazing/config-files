# location of config file 
on mac - "~/.tmux.conf"




# Keywords explained
prefix = 'ctrl+b'

# Installing the package manager 
for plugin manager (tpm) 'git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm'
## Then set the following in your .tmux.conf file
__set -g @plugin 'tmux-plugins/tpm'__ 
At the end of your config file (must be at the end) put the following line
__run '~/.tmux/plugins/tpm/tpm'__
### Installing new packages 
once you have added the relevent line in your config, 
simply do 'prefix + I' __(capital I as in install)__ to fetch plugin 


# Tmux sessions with Tmux Resurrect 
you must explicitly hit a hotkey to store sessions. 
You can do this by 'prefix + (ctrl+s)' to save the session 
This will save the file to '~/.tmux/resurrect'
so now if you kill-server or comeback after restart, 
you can hit 'prefix + (ctrl+r)' to restore the previously saved session 

