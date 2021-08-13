![Sms77.io Logo](https://www.sms77.io/wp-content/uploads/2019/07/sms77-Logo-400x79.png "Sms77.io Logo")

# Sms77 Integration Pack

This StackStorm pack allows integration with [sms77](https://www.sms77.io/) service.

## Installation

`st2 pack install https://github.com/sms77io/StackStorm`

## Configuration

Copy [sms77.yaml.dist](sms77.yaml.dist) to `/opt/stackstorm/configs/sms77.yaml` and edit
it as required.

- ``api_key`` - Your API key - get it in
  the [developer dashboard][https://app.sms77.io/developer].

Dynamic values from the datastore can be used too -
see [documentation](https://docs.stackstorm.com/reference/pack_configs.html).

**Caution** : Remember to tell StackStorm to reload new values after modifying the
configuration in `/opt/stackstorm/configs/` by running `st2ctl reload --register-configs`

## Actions

- **send_sms** - Action which sends an SMS using sms77 API.
  `st2 run sms77.send_sms to=01716992343 text=HI2U from=StackStorm`

### Support

Need help? Feel free to [contact us](https://www.sms77.io/en/company/contact/).

[![MIT](https://img.shields.io/badge/License-MIT-teal.svg)](LICENSE)