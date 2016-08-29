# Connection Manager (socket/HTTP)

The connection manager component, as the name suggests, fills the role of managing connections with clients/vendors.


## Responsibilities / Goals


### Identity

This component should tie into a pre-existing/external Identity service.

### Authentication

This component can optionally authenticate ([not authorize](https://web.archive.org/web/20121014105355/http://www.duke.edu/~rob/kerberos/authvauth.html)) a client.
Multiple mechanisms for authentication will be supported.

### Data Agnostic

Apart from identity and authentication, this layer should not care about the type of data passing through it. It is all streaming binary information for this component.


### Protocol agnostic

The goal is to allow bi-directional communication with clients.

Implementations can use TCP, HTTP2, and websockets. HTTP APIs for vendors may be supported with extensions.
