# 盒子模型
## 1.盒子的实际宽度是内容宽度+padding内边距+border边框。margin不算在里面
没有设置box-sizing时，默认值是content-box;设置的width其实只是内容的宽度，真正盒子的宽度还得自己在加上padding内边距和border边框的宽度。

当设置了box-sizing:border-box;时，设置的width就是盒子的真正的宽度，也就是该width已经是内容宽度+padding内边距+border边框的宽度了。
而padding和border会显示原本设置的宽度，内容宽度会根据实际width进行缩减。