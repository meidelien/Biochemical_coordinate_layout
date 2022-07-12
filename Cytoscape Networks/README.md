# How to format NetworkX cytoscape_data to Cytoscape compliant JSON with fixed node locations using notepad++'s Find & Replace tool

## Step 1 - Replace single quoation marks with doubles

Find what: '
Replace with: "

## Step 2 - Separate x & y coordinate fields

- Find what:., 
- Replace with:,\n"y":

- Find what:"pos": array([
- Replace with: "x":

- Find what:.])
- Replace with:

- Find what:. ,
- Replace with:.,

- Find what:.,
- Replace with:,

- Find what:, 
- Replace with:,\n\t"y":

- Find what:_c", 
- Replace with:_c",\n\t

- Find what:_e", 
- Replace with:e",\n\t

- Find what:.,
- Replace with:,

- Find what:, 
- Replace with:,\n\t"y":

- Find what:. ,
- Replace with:,

## Step 3 - lowercase booleans

- Find what:True
- Replace with:true

- Find what:False
- Replace with:false