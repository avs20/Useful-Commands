# Useful-Commands
This file contains useful commands that I encounter in day to day usage and they get the work done.


1. **list all the subdirectoryies which contain 10 number of files excluding . and ..** 

    ``find . -maxdepth 1 -type d -exec bash -c "echo -ne '{} '; ls '{}' | wc -l" \; | awk '$NF==10'``
