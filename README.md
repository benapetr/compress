# compress
btrfs tool that makes it possible to change the +c flags recursively on existing files

# compress vs btrfs-progs
There are some tricks to perform compression of existing files and folder in more efficient way using btrfs userspace tools,
they are however very hard to use, require you to read incredibly long manuals and require deep knowledge and understanding
of btrfs. They also require you to have superuser rights.

compress is, on other hand, designed for average users, who simply want to enjoy transparent compression on linux just as Windows
users can. You can simply compress whole folder (as long as it belongs to you) with no need for superuser as this:

```
# -r is enough, but shows no progress
compress -vr some_folder
```

# installation
sudo cp src/compress /usr/local/bin
