# ----------------------------- 
# Remaps 
# -----------------------------

# Remap prefix to Control + a
set -g prefix C-a
unbind C-b
bind C-a send-prefix

bind -r h select-pane -L  # move left
bind -r j select-pane -D  # move down
bind -r k select-pane -U  # move up
bind -r l select-pane -R  # move right

# split current window horizontally
bind - split-window -v
# split current window vertically
bind _ split-window -h

# pane resizing
bind -r H resize-pane -L 2
bind -r J resize-pane -D 2
bind -r K resize-pane -U 2
bind -r L resize-pane -R 2

# window navigation
unbind n
unbind p

# Session things
bind-key s choose-session

# Create session
bind C-c new-session

# Find session
bind C-f command-prompt -p find-session 'switch-client -t %%'

# move to last active window
bind Tab last-window        

# clear both screen and history
bind -n C-l send-keys C-l \; run 'sleep 0.1' \; clear-history

# reload configuration
bind r source-file ~/.tmux.conf \; display '~/.tmux.conf sourced'

bind-key -n C-Space resize-pane -Z
