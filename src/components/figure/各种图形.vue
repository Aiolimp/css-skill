<template>
  <div
    class="bruce flex-ct-x"
    data-title="各种图形"
  >
    <div class="icon star"></div>
    <div class="icon arrow"></div>
    <div class="icon pacman"></div>
  </div>
</template>

<style lang="scss" scoped>
.icon {
	display: inline-block;
	position: relative;
	margin-right: 20px;
	width: 0;
	font-size: 0;
}

.star {
	border-left: 50px solid transparent;
	border-right: 50px solid transparent;
	border-bottom: 100px solid red;
}

.star::after {
	position: absolute;
	left: -50px;
	top: 30px;
	border-left: 50px solid transparent;
	border-right: 50px solid transparent;
	border-top: 100px solid red;
	content: "";
}

.arrow {
	margin: 0 40px;
	width: 40px;
	height: 40px;
	background-color: red;
}

.arrow::before {
	position: absolute;
	left: -40px;
	border: solid 20px red;
	border-left-color: transparent;
	content: "";
}

.arrow::after {
	position: absolute;
	right: -40px;
	border: solid 20px transparent;
	border-left-color: red;
	content: "";
}

.pacman {
	border-left: 40px solid red;
	border-right: 40px solid transparent;
	border-top: 40px solid red;
	border-bottom: 40px solid red;
	border-top-left-radius: 40px;
	border-top-right-radius: 40px;
	border-bottom-left-radius: 40px;
	border-bottom-right-radius: 40px;
	width: 0;
	height: 0;
}
</style>