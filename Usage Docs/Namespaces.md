## Supporting Multiple Namespaces

Our implementation of Socket.io on iOS required emitting messages and listening for messages on multiple namespaces. 
We've extended the current implementation and now have an array of supported namespaces which are checked against before parsing messages.

### Notes

Before emitting a message, make sure you're in the required namespace. For additional information on how we deal with this, read the Integration Example.

When listening for a message, make sure that the listener can differentiate between different namespaces. You can find out more about how we deal with this in our Integration Example. 
