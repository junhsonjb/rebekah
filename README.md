# Welcome to Rebekah!

Rebekah is a pet project of mine. It is a data store (currently a key-value store)
written in Rust. The name "Rebekah" is loosely meant to be a play on the data store known
as "Cassandra", which is a fairly well known female name. "Rebekah" is another fairly
well known female name which starts with R, and so the Rebekah data store is named that
because it starts with R and was written in *R*ust. 

## What is Rebekah?
As of now, Rebekah will be a key-value data store modeled after Cassandra. It is essentially a 
Rust version of project that I worked on for my Distributed Systems course, although I may 
decide to change the structure a bit. From a high level, Rebekah can be used as a database that
holds key-value associations and stores them in replicated servers.

## How to Use Rebekah
For now, Rebekah will only work on a single machine using IP addresses that are only accessible
when the machine's internet connection is turned off. The reason for this is so that I can focus on
developing the project without worrying about deployment details such as AWS. At some point, 
I may choose to change this so that it can be run on AWS or some other cloud/distributed service,
but that is currently not the case. The idea is to have some sort of application built, so that 
if and when I choose to place it on AWS (or some other distributed platform) I have an application
to work with and therefore don't need to write the code from scratch (even if I have to make major
changes to it).

Rebekah needs to be run on a machine that is disconnected from
the internet because I intend to use sockets and ports to pass messages between processes.
I do not know if these ports will need to be used by any web connections so I'm playing it safe
by keeping Rebekah "offline" so to speak. If at some point, I learn of a way to build Rebekah so that
it can be run while the machine is connected to the internet connection, I'll fix it and do it that
way. (This would be great because disconnecting internet during development has the potential to 
get very annoying.)

## Disclaimer
This project is intended for _learning purposes only_. At some point, it may become a project
that is ready and able to go into production but that is not the case right now. Please don't use 
this project for anything of any value, unless you want to risk losing it. If that happens, I cannot
be held responsible for any damages.
