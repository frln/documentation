`user` service
==============

The `user` service provides a bunch of data and a few helper functions concerning 
the connected user.

data
----

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Name 
      - Type
      - Description
    * - ``context``
      - ``Object``
      - The user context
    * - ``db``
      - ``Object``
      - Info about the database
    * - ``home_action_id``
      - ``(number | false)``
      - Id of the action used as home for the user
    * - ``isAdmin``
      - ``boolean``
      - Is the user an admin
    * - ``isSystem``
      - ``boolean``
      - Is the user part of the system group
    * - ``lang``
      - ``string``
      - language used 
    * - ``name``
      - ``string``
      - Name of the user
    * - ``partnerId``
      - ``number``
      - Id of the partner instance of the user
    * - ``tz``
      - ``string``
      - The timezone of the user
    * - ``userId``
      - ``number``
      - Id of the user
    * - ``userName``
      - ``string``
      - Alternative nick name of the user

functions
---------

.. js:function:: updateContext(update)

    :param object update: the object to update the context with

    update the context with the given object

.. js:function:: removeFromContext(key)

    :param string key: the key of the targeted attribute

    remove the value with the given key from the context

.. js:function:: hasGroup(group)

  :param string group: the group to look for

  :returns: `boolean` is the user in the group

  check if the user is part of a group




