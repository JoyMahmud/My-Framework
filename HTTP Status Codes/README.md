# What do the HTTP status codes 401, 403, 404 and 500 mean?

## What is an HTTP status code?

For every request from a webbrowser the server responds with a status code. If there was a error, you can get additional information about the error. You can find the most frequent error codes and a brief description in the list below.




### HTTP Error 401 Unauthorized

The 401 status code indicates that the HTTP request has not been applied because it lacks valid authentication credentials (usually username and password) for the target resource. If the request included authentication credentials the 401 response indicates that authorization has been refused for those credentials. Please check if your username and password are correct.



### HTTP status 403 Forbidden

This is a permissions issue. You often encounter this error when no index file (.htm, .html or .php) is present and the directory listing is off for a folder in the Web space (Line "Options -Indexes" in a .htaccess file). Sometimes user authentication was provided, but the authenticated user is not permitted to view the content of the folder or file. Other times the operation is forbidden to all users. Sometimes this error occurs if there are too many connections at the same time. The easyname support team can explain you this issue in depth.



### HTTP status 404 Not Found

This error message is shown when a site or folder on a server are requested but cannot be found at the given URL. Please check your input.



### HTTP status 500 Internal Server Error

This is a "catch all" status for unexpected errors. It is a server side error message common causes of this are eg. misconfigured .htaccess files or PHP errors, which you can check in the File php_error.log on your Webhost. You can find the php_error.log file in the /log/ directory - this directory can be found on the same level as your /html/ directory



### HTTP status 503 Service unavailable

This means, that the server is currently unavailable or the server is overallocated. You can check the file php_error.log as described for the status code 500.
Should you not find helpful error messages in the logfile, please try changing the session_cache to the option filesystem, you can do this in the easyname control panel if you navigate to [My Hosting]>>[PHP settings] and click the link "Settings". Please note that this change will take up to 15 minutes to take effect, so please try waiting 15 minutes before trying to call up your site and refresh it.
