# CSS position属性
## 1.position的属性值:
static      
```
当position没有设置时，默认为static。
```
relative    
```
relative是相对定位，相对于正常static的定位，相对于原位置的移动。
```
absolute
```
相对于非static的父节点进行的移动
```
fixed
```
相对于浏览器进行的移动
```
sticky
```
是粘性定位，是介于relative和fixed的
```
## 2.position作用
进行定位
## 3.position属性值分析
### 1.position:static
当没有设置position的时候，文档默认为static。设置为static后，使用left,right,top,bottom进行位置的变化均无效。
### 2.position:relative
position设置为relative时，left,right,top,bottom是相对于当前正常static进行的偏离。relative是相对定位，相对于正常static的定位，相对于原位置的移动。
### 3.position:absolute
position设置为absolute时，该节点的left,right,top,bottom是相对于非static的父节点进行的移动。所以想要absolute有效，要给相对应的父节点设置relative、absolute或fixed.
### 4.position:fixed
position设置为fixed时，该节点的left,right,top,bottom是相对于浏览器进行的移动。而不是相对于前面的元素，所以当屏幕滚动时，该节点的位置还是相对于浏览器是不变的。fixed是浏览器绝对定位。
### 5.position:sticky
position设置为sticky时，是粘性定位，是介于relative和fixed的。relative是相对于static正常的位置进行的定位，fixed是相对于浏览器进行的定位。
要配合滚动，滚动前，该盒子节点是相对于正常static的位置(margin-top)；滚动时，该盒子节点是相对于浏览器的位置(top,top配合滚动）；滚动回原来的位置，该盒子又回到相对正常static的位置。