# patches
Patches for software I use.

# sxhkd
- mouse_support.patch
Implement mouse support via the socket method.
Mouse events are written as messages across a socket.

- mouse_support_2.patch
Implement mouse support via the `!` modifier on button{1-5}.
Mouse events work as so:
```
mod1 + !button1
    printf "%d %d %b\n" "$(pfw)" | xargs wmv
```
This is currently unclean, and I will do my best to improve it.
