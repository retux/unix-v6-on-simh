Unix 6th edition from BTL
=========================

This is distributed for educational purposes, for anyone that wishes to take a glimpse on a 
software that is a huge historical and technical contribution.

Hardware emulation used is provided by simh. Thanks to Bob Supnik and other contributors to simh open
source project.
On Debian and derivatives it can be installed by running:

  # apt-get install simh

And then the pdp11/40 with Unix 6th edition can be booted up by running:

  $ pdp11 boot.ini


  PDP-11 simulator V3.8-1
  Disabling XQ
  Listening on port 1106 (socket 7)
  @unix

See that @unix is the kernel to be booted up.



Step by step recipe can be found on this url:

http://a.papnet.eu/UNIX/v6/installation

If you follow those detailed steps this installation can be reproduced.
This package also includes the original kernel recompilesd as described in to how to,
that allows multi-user operations by running:
  
  $ telnet localhost 1106

ES: Paso a paso puede encontrarse en la siguiente url:

http://a.papnet.eu/UNIX/v6/installation

Se puede hacer paso a paso cada uno de los pasos, incluso recompilar el kernel para tener las ttys
via telnet.
Eso es practico para multi-usuario y cada usuario puede conectarse a un tty corriendo:

  $ telnet localhost 1106

Para iniciar la pdp-11 emulada 

  $ pdp11 boot.ini


  PDP-11 simulator V3.8-1
  Disabling XQ
  Listening on port 1106 (socket 7)
  @unix

Nota: el el prompt de comando "unix" es el nombre del kernel que vamos a iniciar.
