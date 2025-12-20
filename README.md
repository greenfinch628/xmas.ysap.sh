Bash ASCII Christmas Tree
=========================

Print a super fancy Christmas tree in your terminal WITH an animated light show!
Merry Christmas!

![screenshot](tree.gif)

Usage
-----

Run it right now with `curl`:

```
curl xmas.ysap.sh | bash
```

See previous years with:

```
curl xmas.ysap.sh/2025 | bash
curl xmas.ysap.sh/2024 | bash
```

View it in your browser:

https://xmas.ysap.sh

Clone the repo and run it locally:

```
./2025-ascii-christmas-tree
./2024-ascii-christmas-tree
```

Arguments
---------

The 2025 version of the script allows arguments to be passed in - you can see
the usage message with:

```
curl -sS xmas.ysap.sh/2025 | bash -s -- -h
```

And modify some arguments with:

```
curl -sS xmas.ysap.sh/2025 | bash -s -- -s .1 -c '._-'
```

Videos
------

Creating 2024: https://www.youtube.com/watch?v=NENq-G2PsTo

License
-------

MIT License
