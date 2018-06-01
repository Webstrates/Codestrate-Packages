<h2>Description</h2>
<p>Adds chat functionality to a codestrate. It is possible to chat with individual persons or on local channel on a codestrate.</p>
<div class="warning"><b>Account required</b>: You need to be logged in to use the chat functionality.</p>
<h2>Usage</h2>
<h3>Local Chat</h3>
<p>To open the local chat select the "Open Local Chat" menu entry. It will open a chat window for the current codestrate. The messages of the local chat are stored in the HTML of a codestrate.</p>
<h3>Direct Chat</h3>
<p>To open a direct chat select the "Open Direct Chat" menu entry. You need to enter the userId of a user to start a chat (e.g. "example:github"). Direct chat messages are stored within the messages API of Webstrates.</p>
<div class="danger"><b>Storage time</b>: As messages are cleared up by webstrates, direct messages are only available for 30 days.</p>
<h3>Deleting Chats</h3>
<p>Chat messages chat be deleted individually by right-clicking on them or by selecting the "Delete Chat" button in the header of a chat. Deleting messages from the local chat deletes them for all users. Deleting messages from a direct chat only deletes them for the user who deletes it, <b>the other chat-partner still has all the messages</b>.<br></p><h3>Avatars</h3><p>If the Avatars package is installed, a chat can be started right from the avatar button.</p>
<h2>TODO</h2>
<p>
  <ul>
    <li>Add notifications</li>
    <li>Fix Bugs</li>
    <li><strike>Better Styling</strike></li>
    <li><strike>Detect own user in local chat</strike></li>
    <li><strike>Delete Chat-History</strike></li>
    <li><strike>Show date and time</strike></li>
  </ul>
</p>

# Properties

| Property | Value |
| :--- | :--- |
| Name | Chat |
| ID | xXeazcuk |
| Version | 0.3 |
| Description | Adds chat functionality to a codestrate. |
| Tags | `collaboration` |
| Assets | `interact.min.js` |
| Dependencies | - |
| Changelog | `{"0.3":"Deletion of single messages.","0.2":"Fixed creation of chats.","0.1":"Initial version."}` |