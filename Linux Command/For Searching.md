1. locate = This command will go through entire file system . This uses database which is updated once a day.
    syntax for locate = locate aircrack-ng
2. whereis (for binary files) = returns not only the binary file but also the source and man page if available
3. where = returns the location of the binary files in the path variable only
4. find = syntax for find = find directory options name  
	for eg = find / -type f (f means ordinary file) -name apache2
	wild cards
	1. ? = used to represent a single character for eg ?at can find cat hat but not what..
	2. [] = used to find the characters used inside it for eg [c,h]at can find cat hat but not what.
	3. * = used to find any character with any length for eg * at can find cat hat and what also.