..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _keystone-assignment:

.. list-table:: Description of assignment configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[assignment]**
     -
   * - ``driver`` = ``None``
     - (String) Entrypoint for the assignment backend driver in the keystone.assignment namespace. Only an SQL driver is supplied. If an assignment driver is not specified, the identity driver will choose the assignment driver (driver selection based on `[identity]/driver` option is deprecated and will be removed in the "O" release).
   * - ``prohibited_implied_role`` = ``admin``
     - (List) A list of role names which are prohibited from being an implied role.
