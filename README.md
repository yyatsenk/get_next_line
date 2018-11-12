The prototype is:
int get_next_line(const int fd, char **line);

• The first parameter is the file descriptor that will be used to read.

• The second parameter is the address of a pointer to a character that will be used
to save the line read from the file descriptor.

• The return value can be 1, 0 or -1 depending on whether a line has been read,
when the reading has been completed, or if an error has happened respectively.

• get_next_line returns its result without ’\n’.

• Calling function get_next_line in a loop will then allow you to read the text
available on a file descriptor one line at a time until the end of the text, no matter
the size of either the text or one of its lines.
