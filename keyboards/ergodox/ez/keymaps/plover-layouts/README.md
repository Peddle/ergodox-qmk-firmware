# How to choose between TX Bolt and NKRO?

Generally, you should prefer TX Bolt over NKRO (N-key rollover). The latter
requires you to have special entries in your Plover dictionary, and emits a
sequence of keypresses to trigger these entry and enable/disable Plover. This
can sometimes get out of sync with whether Plover is enabled, and can cause
unintended behavior if you use try to enable Plover in an application that's
sensitive to errant keystrokes. TX Bolt doesn't send keystrokes and doesn't need
to enable or disable Plover: you can always leave Plover enabled and it will
never interfere.

There are some technical limitations of when you can use each:

* Some devices don't support keyboards that use NKRO. In that case, use TX Bolt.
* You may not have permissions to install the necessary drivers for the TX Bolt
  serial protocol. In that case, use NKRO.

See the READMEs for each of the layouts for more information.
