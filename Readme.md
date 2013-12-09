Introduction
============

_dvbbc_ allows streaming live TV over HTTP to multiple viewers. It is as
simple as a design one can get.

Setup
=====

 1. Install `dvb-apps` and `ffmpeg` for your distribution

 2. [Scan and setup all your channels][scan] using `scan`

 3. Copy the channel configuration to `.tzap/channels.conf`

 4. Run `dvbbc` and visit `http://localhost/`

Notes
=====

When everything is set up, you want to keep it running. You have
countless choices here but I opted for [supervisord][]. I've provided a
sample config file [`dvbbc.ini`][config] if you chose to go with
_supervisord_.

[supervisord]: http://supervisord.org/
[scan]: http://www.linuxtv.org/wiki/index.php/Scan
[config]: dvbbc.ini
