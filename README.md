# Arknights Story Reader

A simple python program that help you convert Arknights raw story data into other readable format.

You can find raw story data in [Kengxxiao/ArknightsGameData](https://github.com/Kengxxiao/ArknightsGameData)

**CN/JP/EN/KR server files tested**

Only support story. Guides, tutorial and pop-up msg in battle are not supported yet.

## usage:

### **New: Method 1**

```
py xlsxconvert.py folderpath
```

Convert all arknights story raw data in given folder into xlsx file.

positional arguments:
  `folderpath`        The folder path of raw story files

**Require openpyxl module, if you haven't installed openpyxl, run the following command first**

```
pip install openpyxl
```

### **Method 2 (No extra module required)**

```
py csvconvert.py path [path ...]
```

Convert arknights story raw data into csv file.

positional arguments:
  `path`        The filepaths or folder of raw story file, separate with space, if the path is folder path, it will try to convert all .txt files into csv

## v1.6
New command to convert all raw story files into one xlsx file.

Now automatically link the image and background to the [Aceship Toolbox CG Gallery](https://aceship.github.io/AN-EN-Tags/akgallery.html)
  
## v1.5
Now automatically link the image and background to the mooncell wiki (doesn't support for earlier event like Grani)

Now support folder path, which will convert all .txt file in the folder

## v1.4
Fix some issues

## v1.3
Now support multiple arguments


## v1.2
Fix the encoding issue, now will force encode with utf-8 if UnicodeEncodeError orrured, so there may have some decoding problem when open the csv files with Microsoft Excel.

## v1.1 
Fix the regex to fully match the image in EN server

## v1.0 CSV Convertor 
initial release



**To-do list: (maybe never)**
- json convertor
- link the cg or background image to [Mooncell Wiki](http://ak.mooncell.wiki/w/%E5%89%A7%E6%83%85%E8%B5%84%E6%BA%90%E4%B8%80%E8%A7%88) or [Aceship Toolbox](https://aceship.github.io/AN-EN-Tags/akgallery.html)
- Prettify the output into html or anything looks better.
