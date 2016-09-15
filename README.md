Dinkly Mini Ticket Plugin v1.00
===============================

A small and lightweight support ticket system for your Dinkly app.

Converted into a Dinkly plugin from https://github.com/andrewvt/MiniTicket


Installation
------------

  1. Move the `mini_ticket` folder into your dinkly project's `plugins` folder

  2. Add the following lines under the `plugins` section of your `config/config.yml` file:

    ```yaml
    mini_ticket:
            apps:
                mini_ticket_admin:
                    base_href: /ticket
                    app_name: MiniTicketAdmin
                    enabled: true
                    default_module: home
    ```

  3. Make sure to give it a database to talk to as well. Place these lines under the `databases` section of your `config/config.yml` file and tweak as needed:

    ```
    mini_ticket:
            host: localhost
            user: root
            pass: root
            name: dinkly_app
    ```

  4. Build the models - at the command line: `php tools/gen_models.php -s mini_ticket -p mini_ticket -i`


License
-------

The Dinkly Mini Ticket plugin is open-sourced software licensed under the MIT License.


Contact
-------

  - lewsid@lewsid.com (github.com/lewsid), andrew@bluehousegroup.com (github.com/andrewvt)
