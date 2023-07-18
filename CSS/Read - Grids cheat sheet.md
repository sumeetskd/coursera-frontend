**Grids and flexbox cheat sheet**

Note: ‘|’ stands for alternatives or OR.

**Grid**

The syntax for creating a grid:

selector{
    display: grid; /* or inline-grid */
}
Grid shorthand consists of the following properties with default values:

**grid**

A grid will allow you organize the various elements on your page. 

**grid-template-rows: none**

This feature allows you configure your elements so that they are organized similarly to rows on a table. 

**grid-template-columns: none**

This feature allows you configure your elements but with this setting the elements are organized like columns on a table. 

**grid-template-areas: none**

This feature allows you configure the names of a grid and how they sit in relation to one another. 

**grid-auto-rows: auto**

Default setting for all row sizes that have not been explicitly configured. 

**grid-auto-columns: auto**

Default setting for all column sizes that have not been explicitly configured. 

**grid-auto-flow: row**

Default location for rows that are not explicitly allocated. 

**column-gap: normal**

This sets the gap between the columns

**row-gap: normal**

This sets the gap between the rows

**Grid properties for container**

**grid-template-columns**: measurement units | % units |repeat()

Defines the line names, and maintains a constant size of column items. Can accept a range of different measurement sizes.

**grid-template-rows**: measurement units | % units |repeat()

Defines the line names, and maintains a constant size of rows. Can accept a range of different measurement sizes.

**grid-auto-columns**: measurement unit (fixed value for all columns)

Determines the default size for columns that have not been explicitly configured. 

**grid-auto-rows**: measurement unit (fixed value for all rows)

Determines the default size for rows that have not been explicitly configured.

**grid-template**: “header header” auto

This allows you define and maintain named cells on a grid 

“main right” 75vh

This defines two cells named main and right, that have a sizing of 75% of the viewport height. 

“footer footer” 20rem

This defines two cells named footer and footer, that have a sizing of 20 root em (rem). This defines the size in relation to the html font size. 

**Gap**

grid-gap: measurement units

Determines the gap between rows and columns 

grid-column-gap: measurement units

Determines the gap between columns

grid-row-gap: m-unit-1  m-unit-2

Determines the gap between columns

Alignment
justify-items: start | center | end | stretch

Defines the default space that is allot to each item on the grid 

align-items: start | center | end | stretch

Defines the default space related to an item along the grid’s block axis  

place-items: start | stretch /* shorthand for two properties above */

This feature allows you align items with  the block and inline directions.

Justification
justify-content: start | center | end | stretch | space-between | space-evenly | space-around

Defines browser allocation of space to content items in relation to the main-axis 

align-content: start | center | end | stretch | space-between | space-evenly | space-around

Defines browser allocation of space to content items in relation to cross axis and block axis  

place-content: center | start

This feature allows you align items with  the block and inline directions.

Positioning
grid-auto-flow: row | column | dense

This relates to how the items are placed automatically within the grid

grid-auto-columns: measurement units

This relates to the size for columns created without specific size specifications 

grid-auto-rows: measurement units

This relates to the size for rows created without specific size specifications 

Grid properties for items (child)
grid-column: column position /* E.g. 1/2  */

Allows for specifying where on the grid the column is to start. 

grid-column-start: column start position 

This property determines the starting column position an item is placed on a grid. 

grid-column-end: column end position 

This property determines the end column position an item is placed on a grid. 

grid-row: row position /* E.g. 1/2  */

Allows for specifying where on the grid the row is to start. 

grid-row-start: row start position 

This property determines the starting row position an item is placed on a grid. 

grid-row-end: row end position 

This property determines the end row position an item is placed on a grid. 

Justification and alignment
justify-self: start | center | end | stretch

Determines how  an item is positioned inside its aligned container in relation to the appropriate axis. 

align-self: start | center | end | stretch

Aligns an item within a grid area. 

place-self: start | stretch /* shorthand for two properties above */

This setting lets one align and justify an item within a block. 
