ncmultipyng
===========

ncurses-based ping dashboard, implemented in python

Uses ip addresses given on command-line:

	example: ./ncmultipyng 127.0.{1..3}.{1..10}

Display is in color if your terminal allows it (green=ok, red=ko)

It starts in (p)acked display mode (number of columns adapts to terminal width)

	┌ncmultipyng──────────────────────────────────────────────┐
	│127.0.1.1 !!    127.0.1.2 !!    127.0.1.3 !!             │
	│127.0.1.4 !!    127.0.1.5 !!    127.0.1.6 !!             │
	│127.0.1.7 !!    127.0.1.8 !!    127.0.1.9 !!             │
	│127.0.1.10 !!    127.0.2.1 !!    127.0.2.2 !!            │
	│127.0.2.3 !!    127.0.2.4 !!    127.0.2.5 !!             │
	│127.0.2.6 !!    127.0.2.7 !!    127.0.2.8 !!             │
	│127.0.2.9 !!    127.0.2.10 !!    127.0.3.1 !!            │
	│127.0.3.2 !!    127.0.3.3 !!    127.0.3.4 !!             │
	│127.0.3.5 !!    127.0.3.6 !!    127.0.3.7 !!             │
	│127.0.3.8 !!    127.0.3.9 !!    127.0.3.10 !!            │
	│127.0.4.1 !!    127.0.4.2 !!    127.0.4.3 !!             │
	│127.0.4.4 !!    127.0.4.5 !!    127.0.4.6 !!             │
	│127.0.4.7 !!    127.0.4.8 !!    127.0.4.9 !!             │
	│127.0.4.10 !!    127.0.5.1 !!    127.0.5.2 !!            │
	│127.0.5.3 !!    127.0.5.4 !!    127.0.5.5 !!             │
	│127.0.5.6 !!    127.0.5.7 !!    127.0.5.8 !!             │
	└ quit linear packed ─────────────────────────────────1/99┘

You can switch it to (l)inear display mode

	┌ncmultipyng──────────────────────────────────────────────┐
	│127.0.5.6 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.5.7 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.5.8 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.5.9 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.5.10 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.1 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.2 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.3 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.4 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.5 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.6 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.7 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.8 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.9 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.6.10 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	│127.0.7.1 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!│
	└ quit linear packed ───────────────────────────────46/300┘

In both case you can scroll (up/down/pgup/pgdown/home/end).

