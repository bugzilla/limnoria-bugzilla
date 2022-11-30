# Limnoria Bugzilla Plugin

This plugin for Limnoria (Supybot) supports querying Bugzilla installations,
showing details about bugs, and reading bugmails sent from Bugzilla to show
updates in an IRC channel. It supports working with multiple Bugzilla
installations and can work across many channels and networks.

The main commands you'll be interested in at first are "Bugzilla add", and
then "query" and "bug". Then you should set the
plugins.Bugzilla.defaultBugzilla configuration parameter.

You will probably also want to enable plugins.Bugzilla.bugSnarfer, which
catches the words "bug" and "attachment" in regular IRC conversation and
displays details about that bug or attachment.

The plugin has lots and lots of configuration options, and all the
configuration options have help, so feel free to read up after loading the
plugin itself, using the "config help" command.

Note that if you set it up to parse incoming bugmail, the bot will need WRITE
access to your mail spool *directory* (not just the spool file). This is
because of procmail-compatible file locking and temp files. Often you can do
this by adding the bot user to the 'mail' group.

Report bugs at https://bugzilla.mozilla.org/enter_bug.cgi?product=Bugzilla&component=Limnoria-Bugzilla%20IRC%20Bot

Contribute fixes by filing a pull request at
https://github.com/bugzilla/limnoria-bugzilla