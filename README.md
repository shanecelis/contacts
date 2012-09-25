README for contacts
===================

The utility `contacts` provides command line access to view and search
all records in the AddressBook database.

Build
-----

To build from the source distribution, run:

    $ make

Install
-------

    $ sudo make install

Uninstall
---------

    $ sudo make uninstall

Examples
--------

Here are a few examples:

    $ contacts -h
    usage: contacts [-hHsmnlS] [-f format] [search]
          -h displays help (this)
          -H suppress header
          -s sort list
          -m show me
          -n displays note below each record
          -l loose formatting (does not truncate record values)
          -S strict formatting (does not add space between columns)
          -f accepts a format string (see man page)

    This utility displays contacts from the AddressBook database.

    $ contacts
    NAME                  PHONE        IM                  EMAIL                    
    Kim Jong Il           +82-(001)385 License2KimJongill  mrill@axisofevil.org
    George W Bush         202-276-4300 Bush43              big.dubya@whitehouse.gov
    [...]

    $ contacts bush
    NAME                  PHONE        IM                  EMAIL                    
    George W Bush         202-276-4300 Bush43              big.dubya@whitehouse.gov

    $ contacts -f "%n %w" mrill
    NAME                  HOMEPAGE
    Kim Jong Il           http://www.livejournal.com/users/kim_jong_il__/

For more information and details, see the man page.  :)

Contributions, patches, ideas, and criticisms are welcome.

-shane (at) gnufoo (dot) org
