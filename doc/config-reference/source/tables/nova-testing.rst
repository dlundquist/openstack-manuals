..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _nova-testing:

.. list-table:: Description of testing configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[DEFAULT]**
     -
   * - ``fake_network`` = ``False``
     - (Boolean) This option is used mainly in testing to avoid calls to the underlying network utilities.
   * - ``monkey_patch`` = ``False``
     - (Boolean) Determine if monkey patching should be applied.

       Related options:

       * ``monkey_patch_modules``: This must have values set for this option to have any effect
   * - ``monkey_patch_modules`` = ``nova.compute.api:nova.notifications.notify_decorator``
     - (List) List of modules/decorators to monkey patch.

       This option allows you to patch a decorator for all functions in specified modules.

       Possible values:

       * nova.compute.api:nova.notifications.notify_decorator

       * nova.api.ec2.cloud:nova.notifications.notify_decorator

       * [...]

       Related options:

       * ``monkey_patch``: This must be set to ``True`` for this option to have any effect
