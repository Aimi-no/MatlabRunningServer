# MatlabRunningServer
Example for a server in python running Matlab functions using command line


Requires: flask (pip install flask), pyopenssl (pip install pyopenssl)


Server is located in matlap_server.py and an example sending a POST request is in matlab_test.py.The tested Matlab function is located in test.m. Change the URL in the matlab_test file to the IP running on your server.

Generate certificate and key: openssl req -x509 -newkey rsa:4096 -nodes -out cert.pem -keyout key.pem -days 365


Run example: python matlab_server.py  --matlab_path "C:/Program^ Files/MATLAB/R2020a/bin/matlab.exe" --matlab_script_folder D:/Documents --matlab_function test


Run test example: python matlab_test.py
