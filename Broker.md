# Broker

A broker can be seen as a special router + translator which may or may not have an arbitrarily complex [Backend (bots/webserver)](./Backend.md) behind it.

### Responsibilities / Goals

The lines between a broker and a backend are somewhat blurred at the moment, clearer specs will keep emerging as we work through the use cases.

Current consensus is to have ACL implemented separately and plugged in at various layers of the stack based on a standard permissions model.

If you have something to add, open an issue or send a PR to the [Auth](./Auth.md) page

### Authorization and Permissions.
Each topic needs to be treated as a resource and appropriately ACL has to be implemented.

