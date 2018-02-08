# Sahil Yadav

# Administration Assessment
****

1.	There were many approaches that I came across:

	* We can `rsync` the file with some other machine/rsync daemon itself. This will keep copy of file updated whenever we `rsync` the two hosts. See `man rsync` for more.
	* We can use some [DVCS](https://en.wikipedia.org/wiki/Distributed_version_control) which can maintain a stable copy at every point of time.
	* Though this is a bit complicated (and a bit impractical for what I think), but if possible, we can save a deep copy of our file in [CMOS memory](http://www.pcguide.com/ref/mbsys/bios/comp_CMOS.htm) where the BIOS configuration is stored. This way, the file will be kept safe even if the harddisk gets corrupted. Currently CMOS memory is much less in size (around 64 bytes each), and the data we will be having in a year is around 140 kB (144,000 lines in total assuming 50 characters per line,i.e, 50 bytes constitute one line), it's a bit hard to distribute such amount in the CMOS memory. But we never know what [Moore's law](https://www.britannica.com/topic/Moores-law) has in store for us!

	Since there was no question on the security of content of the file, I have refrained from going on deeper on that aspect. I took help from Google and IRC freenode's `##networking` channel for the last option.

****

2.
