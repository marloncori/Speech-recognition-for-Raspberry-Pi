# Speech-recognition-for-Raspberry-Pi

download those two files and open the shell and unpack sphinxbase with the following command:

tar -xzvf <file name>
  
cd sphinxbase<dir name>
  
  ./configure --enable-fixed
  
  (date and time should be set in the RPi)
  
  now download python-dev and cython if they are not installed yet
  and also pkg-config
  
  now type:
  
  make
 
  sudo make install
  
  now unpack spocketsphinx
  
  tar -xzvf <file name>
  
  cd pocketsphinx
  ./configure
  make
  sudo make install
  
  now edit /etc/ld.so.conf as root
  add
  
  /usr/local/lib
  
  save it and type now:
  sudo /sbin/ldconfig
  
  for the system to find the files.
