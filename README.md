# MintScan_WS
This script uses selenium to grab a png file and pass it to tesseract for text detection. If the uptime falls below
a certain threshold an email is sent to a recipient. At the current settings it takes approximately 22 seconds per 
cycle which can be reduced my intention was to give chrome a good buffer to take a screen shot while debugging. Initially
some basic image processing was attempted, but the raw cropped image data performed perfectly in comparison. The
dictionary is printed to console and is not currently being saved the loop is meant to run continously to monitor
uptime activity. Mintscan currently does not have an api so this avenue was pursued to get data. A headless browser
with bs4 was attempted, but it was not possible to get a full html doc. Future tests will be to parse an entire page
or groups of pages into a DB provided their layouts are the same.
