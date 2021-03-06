### 方法

| 方法名      | 说明          | 参数      |
|---------- |-------------- |---------- |
| on | 事件回调 | (type, callback)1.事件名，2.触发事件时的回调函数；[查看更多](/eleTree/usedocs-event) |
| getChecked | 获取复选框选中的节点信息 | (leafOnly, includeHalfChecked)1.是否只选中叶子节点，默认false，2.是否包括半选节点，默认false |
| setChecked | 设置复选框选中的节点 | (checkArr, isUnCheckAll)1.设置选中项数组，2.是否先清空原有的选中项，默认true |
| unChecked | 取消复选框选中的节点 | (unCheckArr)1.取消选中的节点数组；不传参数则默认清空所有选中项；<span style="color: #ff4200">注意：如果父子节点都是选中的，则如果要取消子节点，需要先取消父节点，即父节点必须包含在数组中</span> |
| getRadioChecked | 获取单选框选中的节点信息 | — |
| setRadioChecked | 设置单选框选中的节点 | (checkArr, isUnCheckAll)1.设置选中项数组，2.是否先清空原有的选中项，默认true |
| unRadioChecked | 取消单选框选中的节点 | (unCheckArr)1.取消选中的节点数组；不传参数则默认清空所有选中项 |
| expandAll | 展开所有节点 | — |
| unExpandAll | 合并所有节点 | — |
| append | 添加子节点 | (id, array)1.查找需要添加的节点id，2.添加的子节点数据数组；id传null或空字符串则会添加到根节点 |
| updateKeySelf | 更新当前节点数据 | (id, object)1.查找需要修改的节点id，2.需要修改的数据 |
| remove | 删除节点数据 | (removeArr)1.需要删除的节点id数组(可以移除多个节点) |
| insert | 在某个节点前后插入数据 | (id, array, type)1.查找需要添加的节点id，2.需要添加节点数据数组，3.类型，在当前节点前插入还是节点后插入，可选参数('before','after')，默认节点前 |
| reload | 重新渲染树节点 | (options)1.传入object，参数初始参数一致 |
| search | 搜索树节点 | (value, callback)1.需要搜索的文本信息，2. 传入的搜索条件，函数返回值为true则显示该节点；[查看更多](/eleTree/demo-search) |
| getAllNodeData | 获取所有节点数据 | — |