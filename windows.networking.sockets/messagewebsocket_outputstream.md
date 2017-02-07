---
-api-type: winrt property
---
 If the websocket instance has been explicitly closed (via delete, **Dispose**, or **Close**) or implicitly closed (fallen out of scope), [FlushAsync](../windows.storage.streams/ioutputstream_flushasync.md) throws an **RO_E_CLOSED** exception.
 If the IOutputStream object associated with the websocket has been explicitly closed (via delete, **Dispose**, or **Close**) or implicitly closed (for example, by disposing of a [DataWriter](../windows.storage.streams/datawriter.md) instance before calling [DetachStream](../windows.storage.streams/datawriter_detachstream.md) on it), [FlushAsync](../windows.storage.streams/ioutputstream_flushasync.md) throws an **RO_E_CLOSED** exception.
 If the websocket is not connected yet ([ConnectAsync](messagewebsocket_connectasync.md) has not been called), then [FlushAsync](../windows.storage.streams/ioutputstream_flushasync.md) throws an **E_ILLEGAL_METHOD_CALL** exception.