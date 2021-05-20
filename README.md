# QA_Bugs

# ID #1

Bug Summary: Duplicate of the incoming message

Precondition: The user is logged in. The “Inbox” folder is open

Steps:

1: Click on the “Write” button.

2: Fill in the fields “To”, “Subject”, and insert text consists of several paragraphs in the text message field. Apply the following formatting types to different parts of the text: bold, underscore, strikethrough, italics, bulleted list, numbered list.

3: Insert valid images (from computer and a link)

4: Click button “Send”.

5: Open the email (by the recipient).

Actual result: Email received. Clicking on it opens a list of two identical emails with appropriate content and all types of formatting.

Expected result: Email received and contains the appropriate content and all types of formatting.

Environment: Microsoft Windows 7; Yandex.browser 21

Service under test: https://mail.yandex.ru

Attachment: https://disk.yandex.ru/i/aY8DAkisyljeKA
____________________________________________________________________________________________________________________________________________
# ID #2

Bug Summary: The selected time ("00:00" for today) is not displayed in the “Delayed message” field

Precondition: The user is logged in. The “Inbox” folder is open.

Steps:

1. Click on the "Write" button.
2. Fill in the fields (“To”, “Subject”, “Message Text”).
4. Next to the "Send" button, click on the “Delayed send” button.
5. Click "Select date and time".
6. Select the date-today, time-00:00 (possible only manually).
7. Click on the “Save” button.

Actual result: In the drop-down list of the "Time" field, the value "00:00" is not active. After making the changes manually, the calendar closes. The “Select Date and Time” field displays today's date and the actual time + 1 minute. The value "00:00" is not displayed in the field.

Expected result: The calendar closes. The "Select date and time" field displays the current date -today and the selected time - "00:00". The message is moved to the “Outgoing” folder.

Environment: Microsoft Windows 7;  Yandex.browser 21

Service under test:  https://mail.yandex.ru

Attachment: https://disk.yandex.ru/i/Fv5Qn2UNnbLvXw

Additional information: When entering the time 00:00 for today in the calendar, the time is entered only from the second time.
_______________________________________________________________________________________________________________________________________________________________
# ID #3

Bug Summary: No "Reference" link in the " Clean folder" pop-up.

Precondition: The user is logged in. The “Inbox” folder is open. Deleted folder is not empty.

Steps:

1. Hover the cursor over the “Deleted Items” folder in the left column and click the “Clear” button.

Actual result: The "Reference" link is missed in the "Clean folder" pop-up.

Expected result: A pop-up appears with the buttons: "Clean", "Cancel" and the link "Reference".

Environment: Microsoft Windows 7; Yandex.browser 21

Service under test: https://mail.yandex.ru

Attachment: https://disk.yandex.ru/i/6pTG_11Apa-f6A
_______________________________________________________________________________________________________________________________________________________________
# ID #4

Bug Summary: The “Create Label” pop-up does not adjust to the screen width.

Precondition: The user is logged in. The “Inbox” folder is open.

Steps:

1. In the left column, click the “Create Label” button.
2. Go to DevTools>Elements. Change the pop-up parameters to the browser window width 1600 px and 1000 px alternately.

Actual result: 
1. With a browser window width of 1600 px – the pop-up width is 432 px, and the height is 297.
2. With a browser window width of 1000 px – the pop-up width is 432 px, and the height is 297.

Expected result:
1. With a browser window width of 1600 px – the pop-up width is 432 px, the height is 295.2.
2. With a browser window width of 1000 px – the pop-up width is 310 px, the height is 212.

Environment: Microsoft Windows 7; Yandex.browser 21

Service under test: https://mail.yandex.ru

Attachment:  
https://disk.yandex.ru/i/t5GcdqLBQEZ-6A

https://disk.yandex.ru/i/AQ1m13L1uucKmg
______________________________________________________________________________________________________________________________________________________________
# ID #5

Bug Summary: Absence of warning message when adding a contact without an email address.

Precondition: The user is logged in. The “Contacts” page is open

Steps:

1. Click on the “Add Contact” button.
2. Fill in the “Name” field with a valid value.
3. Click on the “Add to Contacts” button

Actual result: The contact is added without an email address. There is no validation message.

Expected result: No contact is added. A message appears that you need to enter an email address.

Environment: Microsoft Windows 7; Yandex.browser 21

Service under test: https://mail.yandex.ru

Attachment: https://disk.yandex.ru/i/ZRTE8BqfOQM6nw
_____________________________________________________________________________________________________________________________________________________________
# ID #6

Bug Summary: After adding a new contact, a page with the search results is displayed.

Precondition: The user is logged in. The “Contacts” page is open.

Steps:

1. Click on the “Add Contact” button.
2. Fill in the field for adding an email address with a valid value.
3. Click on the “Add to Contacts” button

Actual result: The popup is closed. Instead of a list of all contacts, a search results page is displayed. The new contact is added to the contact list in the "All" tab.

Expected result: The contact is added to the contact list. The popup is closing. The list of all contacts is open. The All group is highlighted in the left column.

Environment: Microsoft Windows 7; Yandex.browser 21

Service under test: https://mail.yandex.ru

Attachment: https://disk.yandex.ru/i/8l1oQX0Vuo5lXA 
_________________________________________________________________________________________________________________________________________________________________



