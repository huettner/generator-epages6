# ePages 6 Yeoman Generator
Tools and automation for ePages 6 development.

## Precondition

You need a running vm with ePages 6 and shared ``Cartridges`` in your local dev directory.

## Installation

1. Install [NodeJS](https://nodejs.org/)

2. Install Yeoman ``npm install -g yo``

3. Install the ePages 6 generator ``npm install --global https://github.com/ePages-rnd/generator-epages6/archive/master.zip``

4. Go one level above your local ``ePages 6 cartridges`` folder and run ``yo epages6``

5. Follow the instructions

6. (Optional) Install [Chrome Livereload Plugin](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei)

## Available gulp tasks

``default``: Triggers ``build`` and the file ``watch``

``build``: Runs ``make build_ui``

``watch``: Runs file watchers for ``scripts``, ``styles``, ``perl`` and ``html``, based on your settings

``scripts``: Lints your JavaScript file and copies it to the webroot via sftp, triggers livereload

``styles``: Copies the less and css files to the webroot via sftp, triggers livereload

``html``: Runs remote tle linting on the vm, triggers livereload

``perl``: Runs remote perl linting on the vm