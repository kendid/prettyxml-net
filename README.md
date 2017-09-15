# prettyxml

My current workflow (in Microsoft Dynamics AX 2012) includes:

1. Click into the *Infolog*
2. Jump to start/end and mark the whole text (Yes, Ctrl+A doesn't work here)
3. Copy (Ctrl+C)
4. Alt+Tab to Notepad++, maybe open a new file
5. Paste (Ctrl+V)
6. Pretty print XML (Ctrl+Shift+Alt+B) with the XML Tools plugin
7. Change language to XML to make it more readable
8. (Jump to top of file)

This happens multiple times per day when checking whether service methods worked and return the correct XML data. 

To speed it up, this tool should make me able to skip steps 4-8 by:

* Listening to the clipboard for changes
* If new data in the clipboard contains valid XML data:
  * Post it in a memo field in the application form pretty-printed
  * Show the window in front
  * Scroll the memo field to the top

Sometimes there is another step, in which the XML data is BASE64-encoded. If these cases were supported, a couple more steps could be saved. (--> TODO)
