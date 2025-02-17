[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsharoonthomas%2Fpymws.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsharoonthomas%2Fpymws?ref=badge_shield)

=================
Python MWS Client
=================


.. image:: https://img.shields.io/pypi/v/pymws.svg
        :target: https://pypi.python.org/pypi/pymws

.. image:: https://img.shields.io/travis/fulfilio/pymws.svg
        :target: https://travis-ci.com/fulfilio/pymws

.. image:: https://readthedocs.org/projects/pymws/badge/?version=latest
        :target: https://pymws.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status


.. image:: https://pyup.io/repos/github/fulfilio/pymws/shield.svg
     :target: https://pyup.io/repos/github/fulfilio/pymws/
     :alt: Updates



Python client for Amazon Marketplace Web Services (MWS)


* Free software: MIT license
* Documentation: https://pymws.readthedocs.io.


Features
--------

* TODO

Usage
-----

Import the package

`from pymws import MWS`

Create a client instance

.. code-block:: python

  client = MWS(
      marketplace="US", merchant_id="1234",
      access_key_id="key", secret_key="secret",
      auth_token="token"
  )

Once you have a client with valid credentials, you can now
call operations.

.. code-block:: python

  start_date = datetime(2020, 1, 20, 10, 30)
  client.orders.list_orders(CreatedAfter=start_date)


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsharoonthomas%2Fpymws.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsharoonthomas%2Fpymws?ref=badge_large)