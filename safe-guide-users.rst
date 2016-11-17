SAFE for Individual Users
=========================

`SAFE <https://safe.epcc.ed.ac.uk/dirac/>`__ is an online user
service management system. Through SAFE, individual users can request
machine accounts, reset passwords, see available resources and track
their usage. All users must be registered on SAFE before they can apply
for an account on the DiRAC systems.

SAFE: Registering, logging in, passwords
----------------------------------------

How to register on SAFE
~~~~~~~~~~~~~~~~~~~~~~~

#. Go to the SAFE `New User Signup
   Form <https://safe.epcc.ed.ac.uk/dirac/signup.jsp>`__
#. Fill in your personal details. You can come back later and change
   them if you wish
#. Click "Submit"
#. You are now registered. Your SAFE password will be emailed to the
   email address you provided. You can then login with that email
   address and password

At this point your account is registered on the SAFE but you do not
have a user account on any of the DiRAC systems. To obtain a machine account on
DiRAC  please follow the instructions below at:

* `How to request a DiRAC system account`_

How to login to SAFE and Overview of Main Page
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Go to the SAFE <https://safe.epcc.ed.ac.uk/dirac/>`__

#. Type in the email address you have registered with
#. Type in your SAFE password
#. Click "Login"
#. You are now on the Main Page and here you can see Menus along the top
   which give access to SAFE functionality

How to change your personal details on SAFE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Your details* and select *Update personal details*
#. Make the changes you wish
#. Click *Commit Update* to save the changes
#. Go back to *Your details* and you will see the revised information

Do not forget the last step, or nothing will happen. Note that your
postal address does not automatically include the name of your
department and institution; if you want these in your postal address,
you must type them again.

How to change your email address on SAFE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Your details* and select *Update email*
#. Enter the new email address and click *Request*

A verification email will then be sent to the new email address. This
email contains a link which you must use to verify your new address. On
acknowledging your new address the change will be committed and you must
use the new email address when logging into SAFE

How to change your SAFE password
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Your details* and select *Change SAFE password*
#. Fill in the boxes and click *Change*

How to reset your SAFE password
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Enter your email address
#. Click *Email*
#. SAFE will mail your password to your email address

SAFE will only mail to email addresses it already knows. But email is
not a secure medium, so if you change your password this way, you should
immediately change it again `from inside the SAFE. <#chpass>`__

Of course, anyone could go to SAFE, type your email address and request
a new password by clicking "Email". If that happens you will receive an
email message out of the blue saying that your password has been
changed. In this case you should certainly change your password again.

How to add an SSH key to your SAFE account
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Some DiRAC systems may require you to register an SSH key in the SAFE
before you can request an account on the system. To do this you will
require a SSH key pair. You upload the *public part* of the key pair
to your SAFE account as follows:

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Your details* and select *Update personal details*
#. Either copy and paste the public part of your SSH key into the
   "SSH Public key" box or use the button to select the public key file 
   on your computer.
#. Click *Commit Update* to save the changes
#. Go back to *Your details* and you will see the revised information

Do not forget the last step, or nothing will happen.

DiRAC Systems: Accounts, passwords
----------------------------------

How to request a DiRAC system account
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The minimum you require to create a DiRAC system account is
a SAFE account and a *Project Code*. You should sign up for a SAFE 
account as described above and Your project's PI or Project
Manager should be able to supply you with the project code.

Additionally, some DiRAC systems also require that you:

* add the public part of a SSH key to your SAFE account to use when
  logging into the system. If this is required for your system, 
  you must upload this to SAFE before requesting an account by
  following the instructions at: `How to add an SSH key to your SAFE account`_

* provide a list of IP addresses that you will connect to the
  system with. You supply these as part of the sign up process
  for a new account.

The following table indicates what is required by each system:

+----------------------+------------------+-------------------+
| System               | SSH Key Required | IP Range Required |
+======================+==================+===================+
| Edinburgh BG/Q       | No               | No                |
+----------------------+------------------+-------------------+
| Durham COSMA         | Yes              | Yes               |
+----------------------+------------------+-------------------+
| Leicester Complexity | No               | Yes               |
+----------------------+------------------+-------------------+
| Cambridge HPCS       | No               | Yes               |
+----------------------+------------------+-------------------+
| Cambridge COSMOS     | No               | Yes               |
+----------------------+------------------+-------------------+

Once you have thesem you should:

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Login accounts* and select *Request login account*
#. Choose the project you want the account for in the "Choose Project
   for Machine Account" box.
#. Choose the system you want the account on by selecting from the
   available systems. (If a system is not available to select it may 
   be because you have not yet added an SSH keyto your account.)
#. You may need to specify an IP adress range from which you wish to
   connect to the specified system.

Now you have to wait for your PI or project manager to accept your
request to register. When this has happened, the systems team are
prompted to create your account on the service machine. Once this has
been done, you will be sent an email. You can then `pick up your
password <#getpass>`__ for the service machine from your SAFE account.

How to reset a password on your machine account
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you still remember your current machine account password, you can
simply log in to the DiRAC system as normal and then use the passwd command

::

    passwd

You will then be prompted to enter your current password, and then your
new password twice.

If you have forgotten your current password, or it has expired, then you
can ask for it to be reset:

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Login accounts* and select the account you need the
   new password for
#. Click *username* which displays details of this service machine
   account.
#. Click *New Login Account Passwd*

Now the systems team will change your password. When this has been done,
you will be informed by email; this means that you can come back to SAFE
and `pick up your new password <#getpass>`__.

How can I pick up my password for DiRAC system account?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wait till you receive the email with your details. Then:

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Login accounts* and you will see your account on the
   service machine listed. Click on the appropriate account.
#. This will display details of your account. Click *View Login Account
   Password* You will need to enter in your SAFE password and then click
   *view*, and you will see your password to the service machine

This password is generated randomly by the software. It's best to
copy-and-paste it across when you log in to the service machine.

After you login, you will be prompted to change it. You should paste in
the password retreived from SAFE again, and then you will be prompted to
type in your new, easy-to-remember password, twice. 

Note that when you change your password on the service machine in this
way, this is not reflected on the SAFE.

User Mailing Options
--------------------

How to view user mailings
~~~~~~~~~~~~~~~~~~~~~~~~~

| All mailings are archived and can be viewed in
  `SAFE <https://safe.epcc.ed.ac.uk/dirac/>`__.
| Please `login to SAFE <#login>`__ and go to the section *View user
  mailings*. Press the *View* button to access the mailings.

How to get added to, or removed from the email mailing list?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Click on the Menu *Your details* click *Update personal details* find
   *Opt out of user emails* field and click it
#. Click *Commit Update*

Do not forget the last step, or nothing will happen.

**Note:** Regardless of whether you are subscribed to the
mailing list, you can still view ALL user mailings which have been sent,
in SAFE. See `here <#mailings>`__ for details.


Tracking and Managing Available Resources
-----------------------------------------

How to check how much time and space are available to you
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__
and Go to the Menu *Login accounts*, select
the *username* which you wish to see details for. You will then see the
information for this account. You will see the quotas for the disk space
(if the project group/system is using these) and how much is in use.

The budget values displayed are updated every morning, and the values
shown for disk use are updated four times a day. For this reason, all
these values may not be completely up-to-date. If there is a lot of
activity in your project, the numbers shown could be significantly
different from from the current ones.

How to review the use you have made of the service, or the activity of the service as a whole
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Service information* and select *Report Generator*
#. Select the report you wish to run and the format you want the output
   in (web, PDF, CSV, XML) by clicking the appropriate icon in the list.
#. Complete the required information in the form: this will usually
   consist of at least a date range to analyse and may have other
   options depending on the report you are running.
#. Click *Generate Report*

If you are a PI or Project Manager, you will have access to additional
reports to generate information on whole projects or groups as well as
your own usage and the usage of the service as a whole.

Miscellaneous
-------------

How to check the queries you have submitted to the helpdesk
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Login to SAFE <https://www.epcc.ed.ac.uk/dirac/>`__. Then:

#. Go to the Menu *Help and Support* and select *Your support requests*
#. Click the number of a query to check the contents of the query log

This will show you the queries of yours that haven't yet been resolved.
Note that some of the internal correspondence about a query will not be
shown. You can also use SAFE to submit a query—use *New support
request*.

