<template>
  <div class="bruce flex-ct-x" data-title="树形结构和三角标">
    <ul class="tree">
      <li>项目1</li>
      <li>项目2</li>
      <li class="expand">项目3
        <ul>
          <li>子项3.1</li>
          <li>子项3.2</li>
          <li>子项3.3</li>
        </ul>
      </li>
      <li>项目4
        <ul>
          <li>子项4.1</li>
          <li>子项4.2</li>
        </ul>
      </li>
      <li>项目5</li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>

ul {
	list-style: none;
}

.tree li::before {
	display: inline-block;
	border-width: 6px 10.4px;
	border-style: solid;
	border-color: transparent;
	border-left-color: currentColor;
	width: 0;
	height: 0;
	color: #999;
	content: "";
	transform: translateX(6px);
}

.tree li.expand::before {
	transform: rotate(90deg) translateX(6px);
}

.tree li > ul {
	display: none;
}

.tree li.expand > ul {
	display: block;
}
</style>
