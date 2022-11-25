# After Installing Demo data

In hooks.py add after_install hook as following:

```bash
from import __version__ as app_version


app_name = "ems"
app_title = "Ems"
app_publisher = "RG"
app_description = "event management system"
app_email = "rg@rg.com"
app_licence = "MIT"

fixtures = ["Custom Field"]
after_install = "ems.setup.install.after_install"

```

Then create a setup directory and then create a file named install.py in it.

```bash
~/frappe-bench/apps/ems/ems/setup$ touch install.py

```

Now open install.py and create after_install function. This function will be executed automatically
after the app is installed. So in this function we will write the code to insert data into the doctypes.


In my app’s install.py I have made different functions for entering data in different doctypes. Then
these functions are called in after_install function.

```python
def after_install();
	insert_mainevent_data()
	insert_subevent_data()
```
Now, we will see the individual functions to install data in doctypes.

```python

```

```python

```

And the data is currently picked from the array.

```python

```
