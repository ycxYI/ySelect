# ySelect 使用方法
[查看样式范例](https://ycxyi.github.io/ySelect/)
### 引入常用引用
``` html
<link href="css/font-awesome.min.css" rel="stylesheet" type="text/css">
<link href="css/ySelect.css" rel="stylesheet" type="text/css">
```
>其中font-awesome是~~非必须的~~(全选图标)
---

### html代码
``` html
<select id='m1'  multiple="multiple" >
    <option value="1">文本</option>
</select>
```
>注意 在select中加入 multiple="multiple" ,其中`<optgroup label="组"></optgroup>`是被支持的.
---

### javascript代码
###### 你可以直接用默认模板来生成下拉
``` javascript
$('.demo').ySelect();
```
###### 你也可以自定义参数
``` javascript
$('.demo1').ySelect(
    {
        placeholder: '请先选择一些项目',
        searchText: '搜索',
        showSearch: true,
        numDisplayed: 4,
        overflowText: '已选中 {n}项'
    }
);
```
---

### 参数说明
**参数名称** |**说明**
-|-
**placeholder** |选择框占位符
**searchText** |下拉搜索占位符
**showSearch** |显示搜索 (true/false)
**numDisplayed** |超出数量整合
**overflowText** |超出数量整合文本提示,{n}为数量
