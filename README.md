# a3s_krypta
Dynamic AES cypter, for .bin files --> Generates '.cpp ' file. /* { was created for use with HAVOC C2 } */

# To run the script; --> make sure to have the scripts(a3s_krypta.py & loda.cpp) in the /tmp directory
# The loda.cpp file is needed, so make sure to have it.
  # run command to krypt .bin file
    $ python3 a3s_krypta.py " ~/path-to/.bin "

=========================================================================================
    If you are hit with an error, like this 
-----------------------------------------------------------------------------------------
  Exception has occurred: ModuleNotFoundError
No module named 'Crypto'
  File "C:\Users\VictorMomodu\Desktop\sandbox\scripts\a3s_krypta.py", line 2, in <module>
    from Crypto.Cipher import AES
ModuleNotFoundError: No module named 'Crypto'
------------------------------------------------------------------------------------------
Do --> 
------------------------------------------------------------------------------------------
     $ pip install pycryptodome
   
     $ pip install cryptography
-----------------------------------------------------------------------------------------
  # run command to krypt .bin file
    $ python3 a3s_krypta.py " ~/path-to/.bin "
------------------------------------------------------------------------------------------

# In the /tmp directory, to convert the generated new.loda.cpp file to .dll, run command
    $ x86_64-w64-mingw32-g++ new.loda.cpp --shared --static -o ProService.dll  
  # Ignore the error, run the command again with the argument " -fpermissive "
              $ x86_64-w64-mingw32-g++ new.loda.cpp --shared --static -o custom_file_name.dll -fpermissive
  


