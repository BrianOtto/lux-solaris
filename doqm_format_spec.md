# DOQM map file format specification

### general info
map are saved in text file format, with `.doqm` file extension  
you can edit these levels with any text editor   
the map can be split into two floors using different tiles  

NOTE: text editors don't really use fonts with characters with sqare aspect ratio,  
 so the resulting level might end up looking a little stretched in-game  
with some text editors, you can change text spacing to circumvent the issue  



### tiles
> tiles marked with the ^ character can change height when upper case (move them to ther upper floor)
>    for instance: you can use 'S' instead of 's' if you want the start to be on the 2nd floor

`s` ^ : start  
`f` ^ : finish  

`#` : full-height wall  
`w` : mid-height wall  
`c` : lower ceiling  
`p` : platform between 1st and 2nd floor  
`e` : elevator that takes you to the 2nd floor  
`<space>` : empty space with floor and ceiling  
`-` : completely empty tile  



### here is a very simple example level (size 8x8)
finish is on a elevated platform made with walls (w), where you can't get without the elevator (e)  

```
########
#      #
# s    #
#      #
#      #
#wwweww#
#wwwwwF#
########
```