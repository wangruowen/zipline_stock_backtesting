First, you need to install zipline: http://www.zipline.io/beginner-tutorial.html

1. Install "zipline" backtesting framework: 
    $ pip install zipline
    
2. Install ta-lib for Technical Analysis like Moving Average, etc. http://ta-lib.org 

    $ wget http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz
    
    $ tar xvfz ta-lib-0.4.0-src.tar.gz
    
    $ cd ta-lib-0.4.0
    
    $ ./configure
    
    $ make
    
    $ make install
    
    $ export LD_LIBRARY_PATH="/usr/local/lib:$LD_LIBRARY_PATH"
    
    $ pip install ta-lib
    
3. Install other python libraries like numpy, pandas, matplotlib, etc. 
4. zipline ingest

Then try my script in the terminal:

$ zipline run -f ./buystock.py --start 2013-1-1 --end 2017-3-18 -o buystock_out.pickle
