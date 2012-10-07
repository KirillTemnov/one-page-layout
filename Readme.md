# One page layout for mobile devices

  This simple stylus module provides some kind of grid layout for mobile devices.
  
  At present it have presets for iPhone and iPad devices.
  
  In desktop browsers some classes may be very buggy (e.g. firefox and row-100h, col-100w classes).
  

# Basic classes

  All screen divides to columns and sells, whitch are 12.

  Column sizes provides by classes from `col1` to `col12`.

  Layout also have classes like `col-X`, that means substraction of `X` column sizes from max screen width. 
  
  Note: `col-12` have width 0px!

  Group classes from `hcol1` to `hcol12` and from `hcol-1` to `hcol-12` means same as `col`, except that width are *half of column size* on **tablets** and *same size* on **smartphones**.
  
  For row classes same story, but with height.
  
  When add `-vert` or `-horiz` prefix to col and row dimensions - apply these styles to 
  vertical or horizontal mode accordingly.
  
## list of classes

### dimensions
  X changes from 1 to 12.
  
- `row-100h` -  height 100 % of device height
- `col-100w` -  width  100 % of device width
- `h100` - height 100 % of parent block height
- `w100` - width  100 % of parent block width

- `colX` - element width: X columns
- `col-X` - element width: max device width - X columns
- `hcolX` - element width: X/2 columns
- `hcol-X` - element width: max device width - X/2 columns

- `rowX` - element height: X rows
- `row-X` - element height: max device height - X rows
- `hrowX` - element height: X/2 rows
- `hrow-X` - element height: max device height - X/2 rows

### visibility
- `phone-only` - display element only on smartphones
- `tablet-only` - display element only on tablets
- `tv-only` - display element only on tv, or monitor
- `hires-tv-only` - display element only on hi resolution tv or monitor

- only portrail layout:
  `colX-vert`, `col-X-vert`, `hcolX-vert`, `hcol-X-vert`,
  `rowX-vert`, `col-X-vert`, `hcolX-vert`, `hcol-X-vert`  

- only decktop or landscape layout:
  `colX-horiz`, `col-X-vert`, `hcolX-vert`, `hcol-X-vert`,
  `rowX-horiz`, `col-X-vert`, `hcolX-vert`, `hcol-X-vert`  

### fonts
 
- `huge-font` -- biggest font
- `gigant-font` - font with height equal to h1 height
- `bigger-font` - font with height equal to h2 height
- `big-font` - font with height equal to h3 height
- `medium-font` - font with height equal to h4 height
- `normal-font` - font with height equal to h5 (and all text) height 
- `small-font` - font with height equal to h5 height
- `tiny-font` - smallest font for normal text (sup and sub elements are samller font size)

# usage

 You may put .styl file in static directory, that served by connect, express of flatiron if it
 configured to comple stylus templates on the fly, or just compile it with:
 
   ```bash
   stylus one-page-layout.styl
   ```
   
 

# Thanks to

  Some ideas (and couple styles) was taken form http://lessframework.com

# Licence 
    
  (The MIT License)
  
  Copyright (c) 2012 Temnov Kirill allselead@gmail.com
  
  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
  
  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
  
  THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  

