# tmux.conf
my tmux config



```bash

unbind C-b
set -g prefix C-x

# vim
set -g terminal-overrides ',xterm-256color:Tc'
set -g default-terminal "screen-256color"
set -as terminal-overrides ',xterm*:sitm=\E[3m'

bind h split-window -v
bind v split-window -h
# List of plugins
set -g mode-keys vi
set -g @plugin 'tmux-plugins/tpm'
set -g @plugin 'tmux-plugins/tmux-sensible'
set -g @plugin 'dracula/tmux'
set -g @dracula-show-powerline true
set -g @dracula-git-disable-status true
set -g @plugin 'tmux-plugins/tmux-resurrect'
set -g @plugin 'tmux-plugins/tmux-continuum'
# Other examples:
# set -g @plugin 'github_username/plugin_name'
# set -g @plugin 'github_username/plugin_name#branch'
# set -g @plugin 'git@github.com:user/plugin'
# set -g @plugin 'git@bitbucket.com:user/plugin'

# Initialize TMUX plugin manager (keep this line at the very bottom of tmux.conf)
run '~/.tmux/plugins/tpm/tpm'



```
