Init written in PLT Racket

Linux init written in PLT Racket.

1) Why?    I'd like to see if a systemd alternative is viable and DMD is written in GUILE. Perhaps, one can be written in Racket.

2) How?    rinit and a portion of the racket libraries will need to be loaded into initramfs. rinit will support interpreting configuration scripts written in PLT Racket as well as compiling those scripts to bytecode. This may or may not speed up init, but certainly will lead to an interesting init.

Possible roadmap:
1) vmlinuz -> initramfs -> hooks -> rinit -> userspace
2) vmlinuz -> initramfs -> rinit -> userspace
