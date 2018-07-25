CultureMesh 1.0.0
=================

.. toctree::
    :maxdepth: 3





Base URL
~~~~~~~~

https://www.culturemesh.com/api/v1

ACCOUNTS
~~~~~~~~


Data and actions about CultureMesh accounts.





GET ``/token``
--------------


Summary
+++++++

Get user token.

Description
+++++++++++

.. raw:: html

    Gets user token that can be passed in place of email/password combo for @auth.login_required() routes. Lasts for 600 seconds. To pass user/password credentials, try running "curl -u <email>:<password> <rest_of_command>"


Request
+++++++


Headers
^^^^^^^

.. code-block:: javascript

    email: Email or token for login.
    password: Password for login.


Responses
+++++++++

**200**
^^^^^^^

OK


**405**
^^^^^^^

Invalid input




  
EVENTS
~~~~~~


Data and actions about CultureMesh events.





GET ``/event/{eventId}``
------------------------


Summary
+++++++

Get an event.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        eventId | path | Yes | integer | int64 |  | ID of event to return.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: :ref:`Event <d_0a2398219b5d02ebe69f60d7c2c3a96d>`

**Example:**

.. code-block:: javascript

    {
        "address_1": "somestring",
        "address_2": "somestring",
        "city": "somestring",
        "country": "somestring",
        "date_created": "somestring",
        "description": "somestring",
        "event_date": "2015-01-01T15:00:00.000Z",
        "id": 1,
        "id_host": 1,
        "id_network": 1,
        "region": "somestring",
        "title": "somestring"
    }

**405**
^^^^^^^

Invalid input






GET ``/event/{eventId}/reg``
----------------------------


Summary
+++++++

Get list of registration JSONs for an event.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        eventId | path | Yes | integer | int64 |  | ID of event to fetch attendees.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_register_date | query | No | string | timestamp |  | The latest date of registration, inclusive, to return data for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: array of :ref:`EventRegistration <d_71dac114c491dab3062fc6047c3eb3b6>`


**Example:**

.. code-block:: javascript

    [
        {
            "date_registered": "somestring",
            "id_event": 1,
            "id_guest": 1,
            "job": "somestring"
        },
        {
            "date_registered": "somestring",
            "id_event": 1,
            "id_guest": 1,
            "job": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






POST ``/event/new``
-------------------


Summary
+++++++

Create an event.



Request
+++++++



.. _d_2b9216e0d163465b9ed321ed477ecdd0:

Body
^^^^

The fields needed to create a new event.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        address_1 | No | string |  |  | 
        address_2 | No | string |  |  | 
        city | No | string |  |  | 
        country | No | string |  |  | 
        description | No | string |  |  | 
        event_date | No | string | date-time |  | 
        id_host | No | integer | int64 |  | 
        id_network | No | integer | int64 |  | 
        region | No | string |  |  | 
        title | No | string |  |  | 

.. code-block:: javascript

    {
        "address_1": "somestring",
        "address_2": "somestring",
        "city": "somestring",
        "country": "somestring",
        "description": "somestring",
        "event_date": "2015-01-01T15:00:00.000Z",
        "id_host": 1,
        "id_network": 1,
        "region": "somestring",
        "title": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

Ok


**405**
^^^^^^^

Invalid input






PUT ``/event/new``
------------------


Summary
+++++++

Update an event.



Request
+++++++



.. _d_0a2398219b5d02ebe69f60d7c2c3a96d:

Body
^^^^

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        address_1 | No | string |  |  | 
        address_2 | No | string |  |  | 
        city | No | string |  |  | 
        country | No | string |  |  | 
        date_created | No | string | timestamp |  | 
        description | No | string |  |  | 
        event_date | No | string | date-time |  | 
        id | Yes | integer | int64 |  | 
        id_host | No | integer | int64 |  | 
        id_network | No | integer | int64 |  | 
        region | No | string |  |  | 
        title | No | string |  |  | 

.. code-block:: javascript

    {
        "address_1": "somestring",
        "address_2": "somestring",
        "city": "somestring",
        "country": "somestring",
        "date_created": "somestring",
        "description": "somestring",
        "event_date": "2015-01-01T15:00:00.000Z",
        "id": 1,
        "id_host": 1,
        "id_network": 1,
        "region": "somestring",
        "title": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

Ok


**405**
^^^^^^^

Invalid input




  
LANGUAGES
~~~~~~~~~


API for getting language information from CultureMesh.





GET ``/language/{langId}``
--------------------------


Summary
+++++++

Get language information by id.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        langId | path | Yes | integer | int64 |  | ID of language to get information for.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: :ref:`Language <d_372b28d358a836ab6093b8eb1c0dcb8f>`

**Example:**

.. code-block:: javascript

    {
        "added": 1,
        "id": 1,
        "name": "somestring",
        "num_speakers": 1
    }

**405**
^^^^^^^

Invalid input






GET ``/language/autocomplete``
------------------------------


Summary
+++++++

Get an array of autocomplete entries for a language.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        input_text | query | Yes | integer | int64 |  | Partial input query text.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: array of :ref:`Language <d_372b28d358a836ab6093b8eb1c0dcb8f>`


**Example:**

.. code-block:: javascript

    [
        {
            "added": 1,
            "id": 1,
            "name": "somestring",
            "num_speakers": 1
        },
        {
            "added": 1,
            "id": 1,
            "name": "somestring",
            "num_speakers": 1
        }
    ]

**405**
^^^^^^^

Invalid input




  
LOCATIONS
~~~~~~~~~


API for getting location information from CultureMesh.





GET ``/location/cities/{cityId}``
---------------------------------


Summary
+++++++

Get information about a city.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        cityId | path | Yes | integer | int64 |  | ID of city to get info from.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: :ref:`City <d_05b61264676c0f996797c83316388c45>`

**Example:**

.. code-block:: javascript

    {
        "country_id": 1,
        "country_name": "somestring",
        "feature_code": "somestring",
        "id": 1,
        "latitude": 1,
        "longitude": 1,
        "name": "somestring",
        "population": 1,
        "region_id": 1,
        "region_name": "somestring",
        "tweet_terms": "somestring"
    }

**405**
^^^^^^^

Invalid input






GET ``/location/countries/{countryId}``
---------------------------------------


Summary
+++++++

Get information about a country.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        countryId | path | Yes | integer | int64 |  | ID of country to get info from.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: :ref:`Country <d_c28e540c71d3689bf1e412182fbfee3c>`

**Example:**

.. code-block:: javascript

    {
        "feature_code": "somestring",
        "id": 1,
        "iso_a2": 1,
        "latitude": 1,
        "longitude": 1,
        "name": "somestring",
        "population": 1
    }

**405**
^^^^^^^

Invalid input






GET ``/location/autocomplete``
------------------------------


Summary
+++++++

Get an array of autocomplete entries for a location.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        input_text | query | Yes | integer | int64 |  | Partial input query text.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: array of :ref:`Location <d_2fb3f7808cf0d7285b3083152a08f4fb>`


**Example:**

.. code-block:: javascript

    [
        {
            "city_id": 1,
            "country_id": 1,
            "name": "somestring",
            "region_id": 1
        },
        {
            "city_id": 1,
            "country_id": 1,
            "name": "somestring",
            "region_id": 1
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/location/regions/{regionId}``
------------------------------------


Summary
+++++++

Get information about a region.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        regionId | path | Yes | integer | int64 |  | ID of region to get info from.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: :ref:`Region <d_9fbc6cec29a82ba7aa62f02b0d3f4426>`

**Example:**

.. code-block:: javascript

    {
        "country_id": 1,
        "country_name": "somestring",
        "feature_code": "somestring",
        "id": 1,
        "latitude": 1,
        "longitude": 1,
        "name": "somestring",
        "population": 1
    }

**405**
^^^^^^^

Invalid input




  
NETWORKS
~~~~~~~~


Data and actions about CultureMesh networks.





POST ``/network/new``
---------------------


Summary
+++++++

Create a new network.

Description
+++++++++++

.. raw:: html

    Note: if an id is null, pass -1 instead.


Request
+++++++



.. _d_856cd492f38f4e3963decdc19fe873f8:

Body
^^^^

The fields needed to create a new network.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        city_cur | No | string |  |  | 
        city_origin | No | string |  |  | 
        country_cur | No | string |  |  | 
        country_origin | No | string |  |  | 
        id_city_cur | No | integer | bigint20 |  | 
        id_city_origin | No | integer | bigint20 |  | 
        id_country_cur | No | integer | bigint20 |  | 
        id_country_origin | No | integer | bigint20 |  | 
        id_language_origin | No | integer | bigint20 |  | 
        id_region_cur | No | integer | bigint20 |  | 
        id_region_origin | No | integer | bigint20 |  | 
        language_origin | No | string |  |  | 
        network_class | No | string |  |  | 
        region_cur | No | string |  |  | 
        region_origin | No | string |  |  | 

.. code-block:: javascript

    {
        "city_cur": "somestring",
        "city_origin": "somestring",
        "country_cur": "somestring",
        "country_origin": "somestring",
        "id_city_cur": 1,
        "id_city_origin": 1,
        "id_country_cur": 1,
        "id_country_origin": 1,
        "id_language_origin": 1,
        "id_region_cur": 1,
        "id_region_origin": 1,
        "language_origin": "somestring",
        "network_class": "somestring",
        "region_cur": "somestring",
        "region_origin": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

OK


**405**
^^^^^^^

Invalid input






GET ``/network/{networkId}``
----------------------------


Summary
+++++++

Get a specific network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        networkId | path | Yes | integer | int64 |  | ID of network to return.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: :ref:`Network <d_f8d55f83489eb5cee3aa8747531b439c>`

**Example:**

.. code-block:: javascript

    {
        "city_cur": "somestring",
        "city_origin": "somestring",
        "country_cur": "somestring",
        "country_origin": "somestring",
        "date_added": "somestring",
        "id": 1,
        "id_city_cur": 1,
        "id_city_origin": 1,
        "id_country_cur": 1,
        "id_country_origin": 1,
        "id_language_origin": 1,
        "id_region_cur": 1,
        "id_region_origin": 1,
        "img_link": "somestring",
        "language_origin": "somestring",
        "network_class": "somestring",
        "region_cur": "somestring",
        "region_origin": "somestring",
        "twitter_query_level": "somestring"
    }

**405**
^^^^^^^

Invalid input






GET ``/network/{networkId}/events``
-----------------------------------


Summary
+++++++

Get all events in a network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        networkId | path | Yes | integer | int64 |  | ID of network get events from.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`Event <d_0a2398219b5d02ebe69f60d7c2c3a96d>`


**Example:**

.. code-block:: javascript

    [
        {
            "address_1": "somestring",
            "address_2": "somestring",
            "city": "somestring",
            "country": "somestring",
            "date_created": "somestring",
            "description": "somestring",
            "event_date": "2015-01-01T15:00:00.000Z",
            "id": 1,
            "id_host": 1,
            "id_network": 1,
            "region": "somestring",
            "title": "somestring"
        },
        {
            "address_1": "somestring",
            "address_2": "somestring",
            "city": "somestring",
            "country": "somestring",
            "date_created": "somestring",
            "description": "somestring",
            "event_date": "2015-01-01T15:00:00.000Z",
            "id": 1,
            "id_host": 1,
            "id_network": 1,
            "region": "somestring",
            "title": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/network/{networkId}/post_count``
---------------------------------------


Summary
+++++++

Get the number of posts in a network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        networkId | path | Yes | integer | int64 |  | ID of network to count posts for.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


.. _i_69456f1ed20ff6d5324e9d838b942bd8:

**Response Schema:**

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        post_count | No | integer | int64 |  | 


**Example:**

.. code-block:: javascript

    {
        "post_count": 1
    }

**405**
^^^^^^^

Invalid input






GET ``/network/{networkId}/posts``
----------------------------------


Summary
+++++++

Get all posts in a network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        networkId | path | Yes | integer | int64 |  | ID of network to get posts from.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`Post <d_4587d7015c937cc8850ef7cf34b50ea7>`


**Example:**

.. code-block:: javascript

    [
        {
            "id": 1,
            "id_network": 1,
            "id_user": 1,
            "img_link": "somestring",
            "post_class": 1,
            "post_date": "somestring",
            "post_original": "somestring",
            "post_text": "somestring",
            "vid_link": "somestring"
        },
        {
            "id": 1,
            "id_network": 1,
            "id_user": 1,
            "img_link": "somestring",
            "post_class": 1,
            "post_date": "somestring",
            "post_original": "somestring",
            "post_text": "somestring",
            "vid_link": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/network/{networkId}/user_count``
---------------------------------------


Summary
+++++++

Get the number of users that belong in a network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        networkId | path | Yes | integer | int64 |  | ID of network to count users for.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


.. _i_20a53f7313377acf4b8027336f82fcb6:

**Response Schema:**

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        user_count | No | integer | int64 |  | 


**Example:**

.. code-block:: javascript

    {
        "user_count": 1
    }

**405**
^^^^^^^

Invalid input






GET ``/network/{networkId}/users``
----------------------------------


Summary
+++++++

Get all members of a network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        networkId | path | Yes | integer | int64 |  | ID of network to return members from.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_register_date | query | No | string | timestamp |  | The latest user registration date, inclusive, to users for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`NetworkRegistration <d_b9c9a677898ddf041b0f6082990f540c>`


**Example:**

.. code-block:: javascript

    [
        {
            "id_network": 1,
            "id_user": 1,
            "join_date": "somestring"
        },
        {
            "id_network": 1,
            "id_user": 1,
            "join_date": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/networks``
-----------------


Summary
+++++++

Get a list of all networks.

Description
+++++++++++

.. raw:: html

    Notice: if you are querying for an null parameter, pass -1 instead. 

Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 
        near_location | query | No | string |  |  | A comma-separated list of country_id, region_id, and city_id, in that order. 
        from_location | query | No | string |  |  | A comma-separated list of country_id, region_id, and city_id, in that order. 
        language | query | No | string |  |  | Name of language. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`Network <d_f8d55f83489eb5cee3aa8747531b439c>`


**Example:**

.. code-block:: javascript

    [
        {
            "city_cur": "somestring",
            "city_origin": "somestring",
            "country_cur": "somestring",
            "country_origin": "somestring",
            "date_added": "somestring",
            "id": 1,
            "id_city_cur": 1,
            "id_city_origin": 1,
            "id_country_cur": 1,
            "id_country_origin": 1,
            "id_language_origin": 1,
            "id_region_cur": 1,
            "id_region_origin": 1,
            "img_link": "somestring",
            "language_origin": "somestring",
            "network_class": "somestring",
            "region_cur": "somestring",
            "region_origin": "somestring",
            "twitter_query_level": "somestring"
        },
        {
            "city_cur": "somestring",
            "city_origin": "somestring",
            "country_cur": "somestring",
            "country_origin": "somestring",
            "date_added": "somestring",
            "id": 1,
            "id_city_cur": 1,
            "id_city_origin": 1,
            "id_country_cur": 1,
            "id_country_origin": 1,
            "id_language_origin": 1,
            "id_region_cur": 1,
            "id_region_origin": 1,
            "img_link": "somestring",
            "language_origin": "somestring",
            "network_class": "somestring",
            "region_cur": "somestring",
            "region_origin": "somestring",
            "twitter_query_level": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input




  
POSTS
~~~~~


Data and actions about CultureMesh posts.





POST ``/post/new``
------------------


Summary
+++++++

Create a post.



Request
+++++++



.. _d_6b0ff15b47705062e8abc6b276523ae4:

Body
^^^^

The required fields for a new post.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | No | integer | int64 |  | 
        id_user | No | integer | int64 |  | 
        img_link | No | string |  |  | 
        post_text | No | string |  |  | 
        vid_link | No | string |  |  | 

.. code-block:: javascript

    {
        "id_network": 1,
        "id_user": 1,
        "img_link": "somestring",
        "post_text": "somestring",
        "vid_link": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

Ok


**405**
^^^^^^^

Invalid input






GET ``/post/{postId}``
----------------------


Summary
+++++++

Get a post.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        postId | path | Yes | integer | int64 |  | ID of post to return.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

The post object


Type: :ref:`Post <d_4587d7015c937cc8850ef7cf34b50ea7>`

**Example:**

.. code-block:: javascript

    {
        "id": 1,
        "id_network": 1,
        "id_user": 1,
        "img_link": "somestring",
        "post_class": 1,
        "post_date": "somestring",
        "post_original": "somestring",
        "post_text": "somestring",
        "vid_link": "somestring"
    }

**405**
^^^^^^^

Invalid input






GET ``/post/{postId}/replies``
------------------------------


Summary
+++++++

Get the replies for a post.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        postId | path | Yes | integer | int64 |  | ID of post to get replies for.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

The post object


Type: array of :ref:`PostReply <d_e4a69c9611f7dfccf440ed6f2608a8d2>`


**Example:**

.. code-block:: javascript

    [
        {
            "id": 1,
            "id_network": 1,
            "id_parent": 1,
            "id_user": 1,
            "reply_date": "somestring",
            "reply_text": "somestring"
        },
        {
            "id": 1,
            "id_network": 1,
            "id_parent": 1,
            "id_user": 1,
            "reply_date": "somestring",
            "reply_text": "somestring"
        }
    ]

**404**
^^^^^^^

Post does not exist.


**405**
^^^^^^^

Invalid input






GET ``/post/{postId}/reply_count``
----------------------------------


Summary
+++++++

Get the number of replies for a post


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        postId | path | Yes | integer | int64 |  | ID of post to get reply count for


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


.. _i_80c5c161cf6210307b9b5fba283e8bd7:

**Response Schema:**

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        reply_count | No | integer | int64 |  | 


**Example:**

.. code-block:: javascript

    {
        "reply_count": 1
    }





POST ``/post/{postId}/reply``
-----------------------------


Summary
+++++++

Reply to a post.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        postId | path | Yes | integer | int64 |  | ID of post to reply to.


Request
+++++++



.. _d_c96f844535f94248ed7d4f010c561de4:

Body
^^^^

Fields needed to make a new post reply

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | No | integer | int64 |  | 
        id_parent | No | integer | int64 |  | The ID of the parent post (or post reply?)
        id_user | No | integer | int64 |  | 
        reply_text | No | string |  |  | 

.. code-block:: javascript

    {
        "id_network": 1,
        "id_parent": 1,
        "id_user": 1,
        "reply_text": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

Ok


**405**
^^^^^^^

Invalid input






PUT ``/post/new``
-----------------


Summary
+++++++

Update a post.



Request
+++++++



.. _d_6b0ff15b47705062e8abc6b276523ae4:

Body
^^^^

The required fields for a new post.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | No | integer | int64 |  | 
        id_user | No | integer | int64 |  | 
        img_link | No | string |  |  | 
        post_text | No | string |  |  | 
        vid_link | No | string |  |  | 

.. code-block:: javascript

    {
        "id_network": 1,
        "id_user": 1,
        "img_link": "somestring",
        "post_text": "somestring",
        "vid_link": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

Ok


**405**
^^^^^^^

Invalid input






PUT ``/post/{postId}/reply``
----------------------------


Summary
+++++++

Update a post reply.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        postId | path | Yes | integer | int64 |  | ID of post to update


Request
+++++++



.. _d_c96f844535f94248ed7d4f010c561de4:

Body
^^^^

Fields needed to make a new post reply

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | No | integer | int64 |  | 
        id_parent | No | integer | int64 |  | The ID of the parent post (or post reply?)
        id_user | No | integer | int64 |  | 
        reply_text | No | string |  |  | 

.. code-block:: javascript

    {
        "id_network": 1,
        "id_parent": 1,
        "id_user": 1,
        "reply_text": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

Ok


**405**
^^^^^^^

Invalid input




  
UPLOADS
~~~~~~~




POST ``/uploads/image``
-----------------------


Summary
+++++++

Upload an image to the BlueHost server.

Description
+++++++++++

.. raw:: html

    Uploads image to server. Must pass file in enctype multipart-formdata with key being 'file' and value being the file itself. Acceptable file types are .png, .jpg, and .gif. The file must also be < 2MB.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        file | formData | Yes | file | int64 |  | Image file < 2MB and of type .png, .gif, or  .jpg


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Returns new URL for image.


**405**
^^^^^^^

Invalid file type.


**413**
^^^^^^^

File too large (>= 2MB)




  
USERS
~~~~~


Data and actions about CultureMesh users.





POST ``/user/{userId}/addToEvent/{eventId}``
--------------------------------------------


Summary
+++++++

Add user to an event.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        userId | path | Yes | integer | int64 |  | ID of user to add.
        eventId | path | Yes | integer |  |  | ID of event to add user to.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


**405**
^^^^^^^

Invalid input






POST ``/user/{userId}/addToNetwork/{networkId}``
------------------------------------------------


Summary
+++++++

Add user to a network.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        userId | path | Yes | integer | int64 |  | ID of user to add.
        networkId | path | Yes | integer |  |  | ID of network to add user to.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


**405**
^^^^^^^

Invalid input






POST ``/user/users``
--------------------


Summary
+++++++

Create a new user



Request
+++++++



.. _d_548bb3c7c5f6520fbd080ff28a7a0268:

Body
^^^^

The fields needed to create a new user.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        act_code | No | string |  |  | Not sure what this is.
        email | No | string |  |  | 
        first_name | No | string |  |  | 
        last_name | No | string |  |  | 
        password | No | string |  |  | 
        role | No | integer | int32 |  | 
        username | No | string |  |  | 

.. code-block:: javascript

    {
        "act_code": "somestring",
        "email": "somestring",
        "first_name": "somestring",
        "last_name": "somestring",
        "password": "somestring",
        "role": 1,
        "username": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

OK






GET ``/user/{userId}``
----------------------


Summary
+++++++

Get a particular user.

Description
+++++++++++

.. raw:: html

    Gets a user.

Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        userId | path | Yes | integer | int64 |  | ID of user to return.


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

Ok


Type: :ref:`User <d_08e18281892e92ee31598debae39c7be>`

**Example:**

.. code-block:: javascript

    {
        "about_me": "somestring",
        "act_code": "somestring",
        "confirmed": true,
        "email": "somestring",
        "first_name": "somestring",
        "fp_code": "somestring",
        "gender": "somestring",
        "id": 1,
        "img_link": "somestring",
        "last_login": "somestring",
        "last_name": "somestring",
        "register_date": "somestring",
        "role": 1,
        "username": "somestring"
    }

**405**
^^^^^^^

Invalid input






GET ``/user/{userId}/events``
-----------------------------


Summary
+++++++

Get list of events associated with a user.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        userId | path | Yes | integer | int64 |  | ID of user to return.
        role | query | Yes | string |  | {"enum": ["hosting", "attending"]} | Can be "hosting" or " attending"  
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`Event <d_0a2398219b5d02ebe69f60d7c2c3a96d>`


**Example:**

.. code-block:: javascript

    [
        {
            "address_1": "somestring",
            "address_2": "somestring",
            "city": "somestring",
            "country": "somestring",
            "date_created": "somestring",
            "description": "somestring",
            "event_date": "2015-01-01T15:00:00.000Z",
            "id": 1,
            "id_host": 1,
            "id_network": 1,
            "region": "somestring",
            "title": "somestring"
        },
        {
            "address_1": "somestring",
            "address_2": "somestring",
            "city": "somestring",
            "country": "somestring",
            "date_created": "somestring",
            "description": "somestring",
            "event_date": "2015-01-01T15:00:00.000Z",
            "id": 1,
            "id_host": 1,
            "id_network": 1,
            "region": "somestring",
            "title": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/user/{userId}/networks``
-------------------------------


Summary
+++++++

Get networks a user belongs to.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        userId | path | Yes | integer | int64 |  | ID of user to return.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_registration_date | query | No | string | timestamp |  | The latest registration date, inclusive, in the networks returned. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`NetworkWithJoin <d_114b3c716faa3466a7fa007af334c376>`


**Example:**

.. code-block:: javascript

    [
        {
            "city_cur": "somestring",
            "city_origin": "somestring",
            "country_cur": "somestring",
            "country_origin": "somestring",
            "date_added": "somestring",
            "id": 1,
            "id_city_cur": 1,
            "id_city_origin": 1,
            "id_country_cur": 1,
            "id_country_origin": 1,
            "id_language_origin": 1,
            "id_region_cur": 1,
            "id_region_origin": 1,
            "img_link": "somestring",
            "join_date": {},
            "language_origin": "somestring",
            "network_class": "somestring",
            "region_cur": "somestring",
            "region_origin": "somestring",
            "twitter_query_level": "somestring"
        },
        {
            "city_cur": "somestring",
            "city_origin": "somestring",
            "country_cur": "somestring",
            "country_origin": "somestring",
            "date_added": "somestring",
            "id": 1,
            "id_city_cur": 1,
            "id_city_origin": 1,
            "id_country_cur": 1,
            "id_country_origin": 1,
            "id_language_origin": 1,
            "id_region_cur": 1,
            "id_region_origin": 1,
            "img_link": "somestring",
            "join_date": {},
            "language_origin": "somestring",
            "network_class": "somestring",
            "region_cur": "somestring",
            "region_origin": "somestring",
            "twitter_query_level": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/user/{userId}/posts``
----------------------------


Summary
+++++++

Get list of posts made by a user.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        userId | path | Yes | integer | int64 |  | ID of user to return.
        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

OK


Type: array of :ref:`Post <d_4587d7015c937cc8850ef7cf34b50ea7>`


**Example:**

.. code-block:: javascript

    [
        {
            "id": 1,
            "id_network": 1,
            "id_user": 1,
            "img_link": "somestring",
            "post_class": 1,
            "post_date": "somestring",
            "post_original": "somestring",
            "post_text": "somestring",
            "vid_link": "somestring"
        },
        {
            "id": 1,
            "id_network": 1,
            "id_user": 1,
            "img_link": "somestring",
            "post_class": 1,
            "post_date": "somestring",
            "post_original": "somestring",
            "post_text": "somestring",
            "vid_link": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






GET ``/user/users``
-------------------


Summary
+++++++

Get users.


Parameters
++++++++++

.. csv-table::
    :delim: |
    :header: "Name", "Located in", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 15, 10, 10, 10, 20, 30

        count | query | No | integer |  |  | The number of results to return.  Between 1 and 100. 
        max_id | query | No | integer |  |  | The maximum ID, inclusive, to return data for. 
        near_location | query | No | string |  |  | A comma-separated list of country_id, region_id, and city_id, in that order. 
        from_location | query | No | string |  |  | A comma-separated list of country_id, region_id, and city_id, in that order. 
        language | query | No | string |  |  | Name of language. 


Request
+++++++


Responses
+++++++++

**200**
^^^^^^^

A list of users matching filter.


Type: array of :ref:`User <d_08e18281892e92ee31598debae39c7be>`


**Example:**

.. code-block:: javascript

    [
        {
            "about_me": "somestring",
            "act_code": "somestring",
            "confirmed": true,
            "email": "somestring",
            "first_name": "somestring",
            "fp_code": "somestring",
            "gender": "somestring",
            "id": 1,
            "img_link": "somestring",
            "last_login": "somestring",
            "last_name": "somestring",
            "register_date": "somestring",
            "role": 1,
            "username": "somestring"
        },
        {
            "about_me": "somestring",
            "act_code": "somestring",
            "confirmed": true,
            "email": "somestring",
            "first_name": "somestring",
            "fp_code": "somestring",
            "gender": "somestring",
            "id": 1,
            "img_link": "somestring",
            "last_login": "somestring",
            "last_name": "somestring",
            "register_date": "somestring",
            "role": 1,
            "username": "somestring"
        }
    ]

**405**
^^^^^^^

Invalid input






PUT ``/user/users``
-------------------


Summary
+++++++

Update a user

Description
+++++++++++

.. raw:: html

    Uses the ID given in the JSON object to determine what user tuple to modify, then updates the rest of the fields with the JSON values given. Note that it is impossible to update a user id.


Request
+++++++



.. _d_08e18281892e92ee31598debae39c7be:

Body
^^^^

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        about_me | No | string |  |  | 
        act_code | Yes | string |  |  | Not sure what this is.
        confirmed | No | boolean |  |  | 
        email | Yes | string |  |  | 
        first_name | Yes | string |  |  | 
        fp_code | No | string |  |  | Not sure what this is.
        gender | No | string |  |  | 
        id | Yes | integer | int64 |  | 
        img_link | No | string |  |  | URL of image
        last_login | No | string | timestamp |  | 
        last_name | Yes | string |  |  | 
        register_date | No | string | timestamp |  | 
        role | Yes | integer | int32 |  | 
        username | Yes | string |  |  | 

.. code-block:: javascript

    {
        "about_me": "somestring",
        "act_code": "somestring",
        "confirmed": true,
        "email": "somestring",
        "first_name": "somestring",
        "fp_code": "somestring",
        "gender": "somestring",
        "id": 1,
        "img_link": "somestring",
        "last_login": "somestring",
        "last_name": "somestring",
        "register_date": "somestring",
        "role": 1,
        "username": "somestring"
    }

Responses
+++++++++

**200**
^^^^^^^

OK




  
Data Structures
~~~~~~~~~~~~~~~

.. _d_05b61264676c0f996797c83316388c45:

City Model Structure
--------------------

A city.


.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        country_id | No | integer | bigint20 |  | 
        country_name | No | string |  |  | 
        feature_code | No | string |  |  | Not sure what this is.
        id | Yes | integer | bigint20 |  | 
        latitude | No | number | float |  | 
        longitude | No | number | float |  | 
        name | No | string |  |  | 
        population | No | integer |  |  | 
        region_id | No | integer | bigint20 |  | 
        region_name | No | string |  |  | 
        tweet_terms | No | string |  |  | Not sure what this is.

.. _d_c28e540c71d3689bf1e412182fbfee3c:

Country Model Structure
-----------------------

A country.


.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        feature_code | No | string |  |  | Not sure what this is.
        id | Yes | integer | bigint20 |  | 
        iso_a2 | No | integer |  |  | Not sure what this is.
        latitude | No | number | float |  | 
        longitude | No | number | float |  | 
        name | No | string |  |  | 
        population | No | integer |  |  | 

.. _d_0a2398219b5d02ebe69f60d7c2c3a96d:

Event Model Structure
---------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        address_1 | No | string |  |  | 
        address_2 | No | string |  |  | 
        city | No | string |  |  | 
        country | No | string |  |  | 
        date_created | No | string | timestamp |  | 
        description | No | string |  |  | 
        event_date | No | string | date-time |  | 
        id | Yes | integer | int64 |  | 
        id_host | No | integer | int64 |  | 
        id_network | No | integer | int64 |  | 
        region | No | string |  |  | 
        title | No | string |  |  | 

.. _d_71dac114c491dab3062fc6047c3eb3b6:

EventRegistration Model Structure
---------------------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        date_registered | No | string | timestamp |  | 
        id_event | Yes | integer | int64 |  | 
        id_guest | Yes | integer | int64 |  | 
        job | No | string |  |  | 

.. _d_372b28d358a836ab6093b8eb1c0dcb8f:

Language Model Structure
------------------------

A language.


.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        added | No | integer | smallint |  | Not sure what this is.
        id | Yes | integer | bigint20 |  | 
        name | No | string |  |  | 
        num_speakers | No | integer | int4 |  | 

.. _d_2fb3f7808cf0d7285b3083152a08f4fb:

Location Model Structure
------------------------

A location is defined by a tuple (country_id, region_id, city_id),
where at least one of them must be specified.  Valid locations
are fully specified prefixes of the tuple, since suffixes
can be auto-completed.


.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        city_id | No | integer | int64 |  | 
        country_id | Yes | integer | int64 |  | 
        name | No | string |  |  | 
        region_id | No | integer | int64 |  | 

.. _d_f8d55f83489eb5cee3aa8747531b439c:

Network Model Structure
-----------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        city_cur | No | string |  |  | 
        city_origin | No | string |  |  | 
        country_cur | No | string |  |  | 
        country_origin | No | string |  |  | 
        date_added | No | string | timestamp |  | 
        id | Yes | integer | bigint20 |  | 
        id_city_cur | No | integer | bigint20 |  | 
        id_city_origin | No | integer | bigint20 |  | 
        id_country_cur | No | integer | bigint20 |  | 
        id_country_origin | No | integer | bigint20 |  | 
        id_language_origin | No | integer | bigint20 |  | 
        id_region_cur | No | integer | bigint2 |  | 
        id_region_origin | No | integer | bigint20 |  | 
        img_link | No | string |  |  | 
        language_origin | No | string |  |  | 
        network_class | No | string |  |  | _l - language
 cc - city
 rc - region
 co - country

        region_cur | No | string |  |  | 
        region_origin | No | string |  |  | 
        twitter_query_level | No | string |  |  | 

.. _d_ab706535623118e8e3da8347b72b5f8f:

NetworkFilter Model Structure
-----------------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        languages_origin | No | array of string |  |  | 
        locations_cur | No | array of :ref:`Location <d_2fb3f7808cf0d7285b3083152a08f4fb>` |  |  | 
        locations_origin | No | array of :ref:`Location <d_2fb3f7808cf0d7285b3083152a08f4fb>` |  |  | 

.. _d_b9c9a677898ddf041b0f6082990f540c:

NetworkRegistration Model Structure
-----------------------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | Yes | integer | int64 |  | 
        id_user | Yes | integer | int64 |  | 
        join_date | No | string | timestamp |  | 

.. _d_114b3c716faa3466a7fa007af334c376:

NetworkWithJoin Model Structure
-------------------------------

A Network with the join_date of the user for which this network
was invoked for, e.g., the /user/{userId}/networks call.


.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        city_cur | No | string |  |  | 
        city_origin | No | string |  |  | 
        country_cur | No | string |  |  | 
        country_origin | No | string |  |  | 
        date_added | No | string | timestamp |  | 
        id | Yes | integer | bigint20 |  | 
        id_city_cur | No | integer | bigint20 |  | 
        id_city_origin | No | integer | bigint20 |  | 
        id_country_cur | No | integer | bigint20 |  | 
        id_country_origin | No | integer | bigint20 |  | 
        id_language_origin | No | integer | bigint20 |  | 
        id_region_cur | No | integer | bigint2 |  | 
        id_region_origin | No | integer | bigint20 |  | 
        img_link | No | string |  |  | 
        join_date | No | :ref:`join_date <i_29817ecd92dc2d31be5382e511134cb4>` | timestamp |  | 
        language_origin | No | string |  |  | 
        network_class | No | string |  |  | _l - language
 cc - city
 rc - region
 co - country

        region_cur | No | string |  |  | 
        region_origin | No | string |  |  | 
        twitter_query_level | No | string |  |  | 

.. _i_29817ecd92dc2d31be5382e511134cb4:

**Join_date schema:**


Map of {"key":"timestamp"}

.. _d_2b9216e0d163465b9ed321ed477ecdd0:

NewEvent Model Structure
------------------------

The fields needed to create a new event.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        address_1 | No | string |  |  | 
        address_2 | No | string |  |  | 
        city | No | string |  |  | 
        country | No | string |  |  | 
        description | No | string |  |  | 
        event_date | No | string | date-time |  | 
        id_host | No | integer | int64 |  | 
        id_network | No | integer | int64 |  | 
        region | No | string |  |  | 
        title | No | string |  |  | 

.. _d_856cd492f38f4e3963decdc19fe873f8:

NewNetwork Model Structure
--------------------------

The fields needed to create a new network.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        city_cur | No | string |  |  | 
        city_origin | No | string |  |  | 
        country_cur | No | string |  |  | 
        country_origin | No | string |  |  | 
        id_city_cur | No | integer | bigint20 |  | 
        id_city_origin | No | integer | bigint20 |  | 
        id_country_cur | No | integer | bigint20 |  | 
        id_country_origin | No | integer | bigint20 |  | 
        id_language_origin | No | integer | bigint20 |  | 
        id_region_cur | No | integer | bigint20 |  | 
        id_region_origin | No | integer | bigint20 |  | 
        language_origin | No | string |  |  | 
        network_class | No | string |  |  | 
        region_cur | No | string |  |  | 
        region_origin | No | string |  |  | 

.. _d_6b0ff15b47705062e8abc6b276523ae4:

NewPost Model Structure
-----------------------

The required fields for a new post.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | No | integer | int64 |  | 
        id_user | No | integer | int64 |  | 
        img_link | No | string |  |  | 
        post_text | No | string |  |  | 
        vid_link | No | string |  |  | 

.. _d_c96f844535f94248ed7d4f010c561de4:

NewPostReply Model Structure
----------------------------

Fields needed to make a new post reply

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id_network | No | integer | int64 |  | 
        id_parent | No | integer | int64 |  | The ID of the parent post (or post reply?)
        id_user | No | integer | int64 |  | 
        reply_text | No | string |  |  | 

.. _d_548bb3c7c5f6520fbd080ff28a7a0268:

NewUser Model Structure
-----------------------

The fields needed to create a new user.

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        act_code | No | string |  |  | Not sure what this is.
        email | No | string |  |  | 
        first_name | No | string |  |  | 
        last_name | No | string |  |  | 
        password | No | string |  |  | 
        role | No | integer | int32 |  | 
        username | No | string |  |  | 

.. _d_4587d7015c937cc8850ef7cf34b50ea7:

Post Model Structure
--------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id | Yes | integer | int64 |  | 
        id_network | No | integer | int64 |  | 
        id_user | No | integer | int64 |  | 
        img_link | No | string |  |  | 
        post_class | No | integer |  |  | Not sure what this is.
        post_date | No | string | timestamp |  | 
        post_original | No | string |  |  | Not sure what this is.
        post_text | No | string |  |  | 
        vid_link | No | string |  |  | 

.. _d_e4a69c9611f7dfccf440ed6f2608a8d2:

PostReply Model Structure
-------------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        id | Yes | integer | int64 |  | 
        id_network | No | integer | int64 |  | 
        id_parent | No | integer | int64 |  | The ID of the parent post (or post reply?)
        id_user | No | integer | int64 |  | 
        reply_date | No | string | timestamp |  | 
        reply_text | No | string |  |  | 

.. _d_9fbc6cec29a82ba7aa62f02b0d3f4426:

Region Model Structure
----------------------

A region.


.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        country_id | No | integer | bigint20 |  | 
        country_name | No | string |  |  | 
        feature_code | No | string |  |  | Not sure what this is.
        id | Yes | integer | bigint20 |  | 
        latitude | No | number | float |  | 
        longitude | No | number | float |  | 
        name | No | string |  |  | 
        population | No | integer |  |  | 

.. _d_08e18281892e92ee31598debae39c7be:

User Model Structure
--------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        about_me | No | string |  |  | 
        act_code | Yes | string |  |  | Not sure what this is.
        confirmed | No | boolean |  |  | 
        email | Yes | string |  |  | 
        first_name | Yes | string |  |  | 
        fp_code | No | string |  |  | Not sure what this is.
        gender | No | string |  |  | 
        id | Yes | integer | int64 |  | 
        img_link | No | string |  |  | URL of image
        last_login | No | string | timestamp |  | 
        last_name | Yes | string |  |  | 
        register_date | No | string | timestamp |  | 
        role | Yes | integer | int32 |  | 
        username | Yes | string |  |  | 

.. _d_2edbfbb27a3a12557a660c2edad7c1fd:

UserFilter Model Structure
--------------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        from_location | No | array of :ref:`Location <d_2fb3f7808cf0d7285b3083152a08f4fb>` |  |  | 
        languages | No | array of string |  |  | 
        near_location | No | array of :ref:`Location <d_2fb3f7808cf0d7285b3083152a08f4fb>` |  |  | 

.. _d_7ab4ea77488c0fde90d474ccc5007fed:

verify_account Model Structure
------------------------------

.. csv-table::
    :delim: |
    :header: "Name", "Required", "Type", "Format", "Properties", "Description"
    :widths: 20, 10, 15, 15, 30, 25

        verify_account | No | integer |  |  | 

