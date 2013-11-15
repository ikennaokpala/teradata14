**To install Teradata on a 64 bit Centos based system.**

  - Clone the entire package from the git repo git@gitlab.ukroi.tesco.org:teradata14.git

Change into the TDICU directory and install the rpm version.

Change into the TeraGSS directory and install the rpm version.

Change into the TDODBC directory and install the rpm version.


Change into the /opt/teradata/client/14/ODBC_64/ path directory and check the tdata.so file dependencies.  


    ldd path/tdata.so 

if the dependencies are all ok and well linked then you can go ahead to install unix ODBC is this is not already install.. it is recommended that you install the version within the package.


Change into the UNI ODBC directory and run the following:


  ./configure && make && sudo make install

Next change directory to cliv2 and install the rpm version:

For BTEQ you need to install piom first as follows:

Change into the PIOM directory and install the rpm version:

Next Change into the BTEQ directory and install the rpm version.

FAST export and fast fast follow a simlar pattern like the rest all that is required is to install the respective rpm version and that is it JOB DONE.


