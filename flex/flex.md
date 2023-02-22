# flex
## 1.flex作用
flex是给任意元素设置display:flex之后，让这个元素成为flex容器。能够给他的子元素提供空间分配和对齐能力。
## 2.flex比例
多个盒子时，给这些盒子设置flex:number。如：flex:1;可以让这些盒子按照1:1:1来分配空间
## 3.flex-direction容器属性
```
当没有给元素设置flex-direction时，默认是按行来排列，即默认是flex-direction:row;
```
```
如果我们要设置成按列来排列，可以通过flex-direction:column;来设置
```
```
flex-direction:row-reverse;盒子之间的顺序进行反转
flex-direction:column-reverse;同理
```
## 4.flex对齐
### 4.1justify-content 水平相关（主轴上的对齐方式 x轴)
```
justify-content:flex-start;没有设置justify-content时，也默认为靠着主轴线的左边靠齐
```
```
justify-content:center;/*设置沿着主轴线的居中对齐 */
```
```
justify-content:flex-end;/*设置沿着主轴线的右侧对齐 */
```
```
justify-content:space-between;/*设置沿着主轴线左右两端对齐，且盒子之间的距离相等 */
```
```
justify-content:space-around;/*盒子之间的距离等于左右两侧到盒子的两倍 */
```
```
justify-content:space-evenly;/*盒子之间的距离等于左右两侧到盒子的距离*/
```
### 4.2align-items 垂直相关（交叉轴的对齐方式 y轴）
```
align-items：flex-start;没有设置align-items时，默认为靠着交叉轴的顶部靠齐
```
```
align-items:center;/*设置沿着交叉轴的居中对齐 */
```
```
align-items:flex-end;/*设置沿着交叉轴的底部对齐 */
```
## 5.flex-wrap容器属性
```
flex-wrap:nowrap;当flex容器中的子元素的总宽度大于父元素的总宽度时，设置为nowrap时，项目会强行等分里面的子元素宽度
```
```
flex-wrap:wrap;项目会根据子元素的自身宽度进行排列，如果超出父元素总宽度会自动换行
```