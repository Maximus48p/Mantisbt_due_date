# due_date
 
In the current version Mantisbt 2.22.0 the field of the due_date ticket becomes 'red' when the due_date is expired.

But that is mostly to late!
This solution warns you (default) five and two days before the due_date expires in green and oranje colours.


The code has been tested in Mantisbt version 2.22.0

My first Github project.... hopefully everythings goes well.

STEP 1:
Add 3 lines below in your config_inc.php file;

# When do want to be warned before the due_date expires? Time is mentioned in seconds.
$g_1st_due_date_warning = 432000; # get's color green (default 5 days)
$g_2nd_due_date_warning = 172800; # get's color orange and always less seconds then the 1st warning (default 2 days)

STEP 2: implement the code.


When installed correctly you now will be warned five days before the due_date in green colour,
and two days before in orange colour.
