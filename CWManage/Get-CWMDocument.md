# Get-CWMDocument
## SYNOPSIS
This function will list documents associated with a record.
## SYNTAX
```powershell
Get-CWMDocument [[-RecordType] <Object>] [[-RecordID] <Int32>] [[-page] <Int32>] [[-pageSize] <Int32>] [[-pageID] <Int32>] [<CommonParameters>]
```
## PARAMETERS
### -RecordType &lt;Object&gt;
The type of document you are looking for.

Agreement, Company, Configuration, Contact, Expense, HTMLTemplate, Opportunity, Project, PurchaseOrder,

Rma, SalesOrder, Ticket, ServiceTemplate, ToolbarIcon, Meeting, MeetingNote, ProductSetup, ProjectTemplateTicket,

WordTemplate, Member, PhaseStatus, ProjectStatus, TicketStatus
```
Required                    false
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -RecordID &lt;Int32&gt;
The ID of a RecordType specified
```
Required                    false
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -page &lt;Int32&gt;
Used in pagination to cycle through results
```
Required                    false
Position                    3
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -pageSize &lt;Int32&gt;
Number of results returned per page (Defaults to 25)
```
Required                    false
Position                    4
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -pageID &lt;Int32&gt;
Used in pagination to request a page by id
```
Required                    false
Position                    5
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Get-CWMDocuments -RecordType Ticket -RecordID 1836414

Will return documents associated with a the ticket 1936414
```

## NOTES
Author: Chris Taylor

Date: 8/22/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/manage/rest?a=System&e=Documents&o=GET
