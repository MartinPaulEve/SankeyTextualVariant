# SankeyVariant

This project aims to allow users to visualise textual variants/textual genetics across editions using modifications to D3.js and its Sankey plugin.

![Screenshot](images/2015-12-Sankey.png?raw=true)

# Usage
Examples are provided in variant.html and 3col.html. The associated data files (data.json and 3col.json) demonstrate the encodings needed to draw textual variance flows.

There are three dictionaries within the JSON: nodes, links, and nolink. Nodes should contain all of the named nodes that you wish to draw.

Nodes should be listed by column in the order in which you want them to appear. New columns will appear with the first in each that is a target.

Links should specify links between nodes as well as the weight (value) that the source will donate to the target. This value determines the thickness of the line.

Nolink should specify nodes that are unlinked. The "value" key here specifies the width of the block. The "location" key specifies the column as a zero-indexed array (so the leftmost column is 0, the next is 1, the next is 2 etc.).

# Credits and license
This software builds heavily upon Mike Bostock's Sankey work for D3.js. See the additional information in the licenses folder for more information. It has been modified by and is copyright Martin Paul Eve, 2015. SankeyVariant is released under the MIT license.

