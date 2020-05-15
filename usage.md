# Usage of Sycor.Back2Work
## Scancodes for check in / check out
When you like users to check in into a space by scanning a code with their smartphone, you have to generate a code for each space and fix it somewhere close to the entrance that users may easily check in.

As PowerApps can read different codes ([more Information](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/controls/control-new-barcode-scanner)) you are free to choose your favorite code. However, we recommend using QR codes. Only the title field of a space must be coded, not other information are needed.

When you want to generate all codes for your organization you may export a list of all sites from your SharePoint data source. Open the list btw_site and perform an export to Excel from this list. You can use this list as input for your favorite scancode generation software. It can also be done with Microsoft Word out of the box functionality. One instruction c be found [here](https://support.office.com/en-us/article/add-barcodes-to-labels-495cf789-c9d9-4ea5-8eb9-7299170d4831).

## Detect contacted persons in case of infection
When an employee reports that he is infected and you want to identify with persons that where in contact with the infected employee, you can analyze the content of the SharePoint list btw_locationTrack, where all check in / check out is stored. In this list you can track when a user was checked in to a certain space. We recommend to export the content of this list and make further analysis with external tools like Excel, SQL or PowerBI.