# bscp
Bscp – Secure and efficient copying of block devices

Bscp copies a single file or block device over an SSH connection, transferring only the parts that have changed.
In other words, it handles the edge case where RSync fails.

# Usage
bscp SRC HOST:DEST [BLOCKSIZE] [HASH]

The default BLOCKSIZE is 65536 (64 KiB). The default HASH algorithm is sha1 (SHA-1).
