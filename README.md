# SeleniumWebdriver-with-Ruby
Direct selence commands to act on browser.



# Window Handler - This will work for both pop-up windows & Tabs.
@driver.switch_to.window(@driver.window_handles.first) --- to target parent window/tab
@driver.switch_to.window(@driver.window_handles.last)  --- to target child window/tab

# Get UN & PWD from excel sheets
-- Here first you should know your excel sheet must be in Excel 97-2003 format.
-- Use "spreadsheet" gem
1. Get the spreadsheet
2. Select first page
3. MOve the values to Hash
    book = Spreadsheet.open 'path to/file.xls' => Open book
 		sheet1 = book.worksheet 0 => Select page
		credentials = sheet1.to_h => Get values in  HAsh

