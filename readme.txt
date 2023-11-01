add-on for mass change: NextGenerator

!!! folder must not be on OneDrive but can be on GoogleDrive (G:\)

Options:
  CSV file: <absolute path to csv file w/ values>
  Non-text values to replace [..]: <JSON formated string that shows what string inside the svg file shall be replaced by what column in the csv file>
  File name pattern: %VAR_<name of column in csv file (should be unique)%
  Save in: <absolute path to folder where data shall be generated (must exist)>
  
  calculate pixels: https://pixelcalculator.com/en
  use 300 DPI
  width: 520 +36 +36 (bleed/cut top/bottom)
  height: 791 +36 +36 (bleed/cut top/bottom)
 
  
Example:
  CSV file: G:\My Drive\darkforce\card values min.csv
  Non-text values to replace [..]:
    {"image_from_miyuki":"image_from_default/default.jpg","backcolor":"#ff6700","backcolor2":"#ffa200","icon_1":"icons/icon_1.png","icon_2":"icons/icon_2.png","icon_3":"icons/icon_3.png","icon_4":"icons/icon_4.png","icon_5":"icons/icon_5.png"}
  File name pattern: %VAR_number%
  Save in: G:\My Drive\darkforce\tmp
  
 JSON Format:
  {"key":"value", "key2":"value2", "key3":"value3"}
  key: column in csv
  value: string to be found in svg and to be replaced
  
  
 AI image prompt: a <title> without any characters, anime style