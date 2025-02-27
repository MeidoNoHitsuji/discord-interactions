====================
discord-interactions
====================

**Easy, simple, scalable and modular: a Python API wrapper for interactions.**

.. image:: https://img.shields.io/pypi/dm/discord-py-slash-command.svg
    :target: https://pypi.python.org/pypi/discord-py-interactions/
    :alt: PyPI Monthly Downloads

.. image:: https://img.shields.io/github/license/goverfl0w/discord-interactions.svg
    :target: https://github.com/goverfl0w/discord-interactions/blob/master/LICENSE
    :alt: License

.. image:: https://img.shields.io/pypi/pyversions/discord-py-interactions.svg
    :target: https://pypi.python.org/pypi/discord-py-interactions/
    :alt: PyPI Versions

.. image:: https://img.shields.io/pypi/v/discord-py-interactions.svg
    :target: https://pypi.python.org/pypi/discord-py-interactions/
    :alt: PyPI Version

.. image:: https://readthedocs.org/projects/discord-interactions/badge/?version=latest
    :target: http://discord-interactions.readthedocs.io/?badge=latest
    :alt: Documentation Status

.. image:: https://discord.com/api/guilds/789032594456576001/embed.png
    :target: https://discord.gg/KkgMBVuEkx
    :alt: Discord

----

Ever since December 2019, this open-source project has become the culmination of dedication and research towards figuring out the best way to bring **interactions from Discord to you:** we are an easy, simple, scalable and modular library for Discord interactions.

- Tired of using numerous module dependencies for slash commands and buttons?
- Looking for a compatible library that implements all interactions?
- Itching to get your hands on slash commands, but in a simple manner?

Look no more! The goal of this library is to make all three of these questions go from possibilites to trivial matters.

What can we do?
***************
Our library---inside and out, offers numerous benefits and presents itself as a worthy module in your bot's dependencies:

The base features of our library, built with our API include:

- **Dynamic object data generation**: all event data dispatched from the Gateway is dynamically transformed and generated into two-way serializable JSON objects.
- **Sane rate limiting**: our HTTP client implements pre-emptive rate limit avoidance, so your bot is guaranteed to never hit HTTP ``429``.
- **On-demand cache**: every HTTP request and Gateway event made is cached when needed, so you never have to save information yourself.
- **Simplified data models**: every object presented is accessible as either a raw dictionary/``application/json`` or list of recursive attributes.

Some more unique features that are exclusive to our interactions include:

- **Event-triggered callbacks**: whether a component, application command or interaction response, you'll never need to worry about bridging responses.
- **Dual-way decorator logic**: a decorator can act as both a constructor for an interaction, as well as a callback.
- **API-strict naming**: no more confusion with the naming approach of many libraries; we follow the naming style of interactions from the officially curated Discord Developers documentation.
- **Extensive framework structure**: (**pending in** ``4.1.0``) build your own tools and technologies for our library to develop and integrate community creations.

What do we not offer?
*********************
While we certainly offer a lot of benefits, we unfortunately have our own downsides:

.. note::
   This list is subject to change as time goes on:
   some of these items may be added to the core of
   the library in the future.

- No native cooldown decorator/method.
- Lack of automatic sharding and voice clients.

Where do I start?
*****************
Please check out our `quickstart guide`_ for some basic examples.

How can I contribute?
*********************
Please read up on our `contribution requirements`_ for the project. This open-source project also enforces the `MIT License`_.

This open-source project utilizes the following workflows for development:

#. **pre-commit** ``2.16.0``: the architecture uses this before every commit to format and check for severity/QOL-breaking changes.

   #. **black** ``21.11b1``
   #. **flake8** ``3.9.2``
   #. **isort** ``5.9.3``

#. **Sphinx** ``4.1.2``: all of our documentation is powered off of autogenerated documentation of the Sphinx engine.
#. **colorama** ``0.4.4``: our internal logger uses a customized coloring formatter to make looking for specific conditions easier when running tests.
#. **Conventional Commits** ``1.0.0``: every commit that we make to our branches use the official specification of CC 1.0.0 to make git graphs easier when improving and refining communication between code reviews, Pull Requests and commits.

When can I start?
^^^^^^^^^^^^^^^^^
We also have some extra ground rules about making any specific contributions involving:

- We do not accept abstraction-based requests. (e.g. ``colour`` for ``color``)
- A request has to be approved by at least one developer.
- You must be willing to change/adhere to reviews from participants **where necessary.**

I think I'm all ready!
^^^^^^^^^^^^^^^^^^^^^^
Feel free to begin making `Pull Requests`_ and `Issues`_ on our GitHub!

.. _quickstart guide: https://discord-interactions.rtfd.io/en/latest/quickstart.html
.. _contribution requirements: https://github.com/goverfl0w/discord-interactions/blob/stable/CONTRIBUTING.rst
.. _MIT License: https://github.com/goverfl0w/discord-interactions/blob/stable/LICENSE
.. _Pull Requests: https://github.com/goverfl0w/discord-interactions/pulls
.. _Issues: https://github.com/goverfl0w/discord-interactions/issues
