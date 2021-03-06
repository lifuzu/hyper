Release History
===============

X.X.X (XXXX-XX-XX)
------------------

- Use bundled SSL certificates in addition to the OS ones, which have limited
  platform availability. (`Issue #9`_)
- Connection objects reset to their basic state when they're closed, enabling
  them to be reused. Note that they may not be reused if exceptions are thrown
  when they're in use: you must open a new connection in that situation.

.. _Issue #9: https://github.com/Lukasa/hyper/issues/9

0.0.2 (2014-02-20)
------------------

- Implemented logging. (`Issue #12`_)
- Stopped HTTP/2.0 special headers appearing in the response headers.
  (`Issue #16`_)
- `HTTP20Connection` objects are now context managers. (`Issue #13`_)
- Response bodies are automatically decompressed. (`Issue #20`_)
- Provide a requests transport adapter. (`Issue #19`_)
- Fix the build status indicator. (`Issue #22`_)


.. _Issue #12: https://github.com/Lukasa/hyper/issues/12
.. _Issue #16: https://github.com/Lukasa/hyper/issues/16
.. _Issue #13: https://github.com/Lukasa/hyper/issues/13
.. _Issue #20: https://github.com/Lukasa/hyper/issues/20
.. _Issue #19: https://github.com/Lukasa/hyper/issues/19
.. _Issue #22: https://github.com/Lukasa/hyper/issues/22

0.0.1 (2014-02-11)
------------------

- Initial Release
- Support for HTTP/2.0 draft 09.
- Support for HPACK draft 05.
- Support for HTTP/2.0 flow control.
- Verifies TLS certificates.
- Support for streaming uploads.
- Support for streaming downloads.
