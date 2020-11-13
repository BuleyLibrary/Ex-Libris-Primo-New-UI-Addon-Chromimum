IMPORTANT:  One of the following settings must be set to true in order for the Addon to work:

-- GoToLandingPage
-- AutoSearchISxN
-- AutoSearchTitle


* Distinction between Primo VE and Non-VE *

Check the box for PrimoVE if your library is on Primo VE. Uncheck the box if your library uses the Primo Back Office.

The front-end "New UI" for Primo VE and Primo Back Office (PBO) appear the same, but the HTML structure differs.
For Ex Libris customers on Primo VE, the information about local holdings and availability is inserted directly
into the full record display. For customers using the PBO, this information is instead in a "mashup" iframe.

Because this addon can't access the information within iframes, libraries using the PBO will see two buttons:

1) One to open the holdings, which navigates directly to the source of the mashup iframe.
2) A second to import the location and call number from this webpage.

Libraries on VE will see the import button only, because the addon can obtain the information from the full record.


* Example Values*

For Central Oregon Community College, the URL of the results page of a Primo query for "dogs" in the ILL staff's
preferred tab and scope is:
https://alliance-primo.hosted.exlibrisgroup.com/primo-explore/search?query=any,contains,dogs&tab=default_tab&search_scope=cocc_alma&vid=COCC&offset=0

BaseURL:
* This value is the path of the Primo URL before the ?
* Customers on Primo VE will see "discovery" in the path instead of "primo-explore"
https://alliance-primo.hosted.exlibrisgroup.com/primo-explore/search

DatabaseName:
* This is the value of the "vid" parameter in the URL.
COCC

SearchTab:
* This value is the code of the tab to search, found in the "tab" parameter.
default_tab

SearchScope:
* This is the code of the scope to search within the tab, found in the "search_scope" parameter.
cocc_alma