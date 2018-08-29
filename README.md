#GmailAPI

*This is very similar to the quickstart available from Google. However, this particular version has some added basic functionality such as message lookup and reading.*
 
After you enable the GMAIL API in Ggl Dev Console you will receive a API Key and Client_ID.

Whitelist your HTTP server and OAuth credentials in dev console.

Separate your auth credentials into seperate JS file so there is not accidental upload to GitHub.

I included bootstrap to add a little styling.

jQuery is included to create 'promise' functions that handle re-authentication problems caused by trying to look up Message ID's after initial authentication.

I plan to add functionality to allow for label exploration.


---------------------------------------

After authenticating when page is loaded it will print a list of available 'labels' associated with users account; i.e. 'inbox', 'sent', 'drafts'...


Then a list of labels (I think 100 is the max available at a time..) will be retrieved and listed.

Any label may be selected and entered into the "lookup message Id" search field; which will return a base64 encoded string.
This string is then decoded and displayed in a seperate section.

