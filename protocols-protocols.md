## Protocol

The language used to ask for data to get sent - in either direction - is
called **the protocol**. The protocol describes exactly how to ask the server
for data. Or to tell the server that there is data coming.

The protocols are typically defined by the IETF ([Internet Engineering Task
Force](http://www.ietf.org)), which hosts RFC documents that describe exactly
how each protocol works. How clients and servers are supposed to act and what
to send and so on.

## What protocols does curl support?

curl supports protocols that allow "data transfers" in either or both
directions. We usually also restrict ourselves to protocols which have a "URI
format" described in an RFC or at least is somewhat widely used, as curl works
primarily with URLs (URIs really) as the input key that specifies the
transfer.

The latest curl supports these protocols:

DICT, FILE, FTP, FTPS, GOPHER, HTTP, HTTPS, IMAP, IMAPS, LDAP, LDAPS, POP3,
POP3S, RTMP, RTSP, SCP, SFTP, SMB, SMBS, SMTP, SMTPS, TELNET, TFTP

To complicate matters further, the protocols often exist in different versions
or flavors as well.

## What other protocols are there?

The world is full of protocols, both old ones and new ones. Old protocols get
abandoned and dropped and new ones get introduced. There's never a state of
stability but the situation changes day to day and year to year. You can rest
assured that there will be new protocols added in the list above in the future
and there will be new versions of the protocols already listed.

There are of course already other protocols in existence that curl doesn't yet
support. We are open to accepting more protocols that suit the general curl
paradigms, we just need developers to write the necessary code adjustments for
them.

## How are protocols developed?

Both new versions of existing protocols and entirely new protocols are usually
developed by persons or teams that feel that the existing ones are not good
enough. Something with them makes them not suitable for a particular use case
or perhaps some new idea has popped up that could be applied to improve
things.

Of course nothing prevents anyone from developing a protocol entirely on their
own at their own pleasure in their own backyard, the major protocols are
usually brought to the IETF at a fairly early stage where they are then
discussed, refined, debated and polished and then eventually hopefully turned
into a published RFC document.

Software developers then read the RFC specifications and deploy their code in
the world based on their interpretations of the words in those documents. It
sometimes turn out that some of the specifications are subject for vastly
different interpretations or sometimes the engineers are just lazy and ignore
sound advice in the specs and still deploy something that isn't adhering.
Writing software that interoperates with other implementations of the
specifications can therefore end up to be hard work.

## How much do protocols change?

Like software, protocol specifications are frequently updated and new protocol
versions are created.

Most protocols allow some level of extensibility and makes new extensions
showing up over time, extensions that make sense to support.

The interpretation of a protocol sometimes change even if the spec remains the
same.

The protocols mentioned in this chapter are all "Application Protocols", which
means they are transferred over more lower level protocols, like TCP, UDP and
TLS. They are also themselves protocols that change over time, get new
features and get attacked so that new ways of handling security etc forces
curl to adapt and change.

## About adhering to standards and who's right

TBD