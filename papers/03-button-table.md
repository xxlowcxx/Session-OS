# The button table

The virtual OS keeps its own buttons. Each one pulls the matching control on the phone. The phone is the only thing actually moving. The session is the puppet. The host holds it.

| Virtual button | Host equivalent |
| --- | --- |
| Touch, key, volume | The host's input events |
| Draw the screen | A window or surface the host owns |
| Read and write files | A folder the host already allows |
| Open the network | The host's sockets |
| Play sound | The host's audio session |
| Shut down the virtual OS | Stop that process |

Each button has one of three outcomes, with a separate row for Android and for iOS:

- Do the host action.
- Do it inside the session.
- Hide it.

A button with no finger on that phone is hidden, not broken. iOS gives an app fewer fingers than Android. Some Linux buttons have no iOS string to pull. They stay inside the session or they stay hidden.

Boot, the kernel, and the signature check have no finger. Nothing in the table reaches them.
