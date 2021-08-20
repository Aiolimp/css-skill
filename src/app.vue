<template>
	<div class="index-page">
		<div class="header flex-ct-y">
			<h1>
				<span class="gradient">Aiolimp CSS</span>
			</h1>
		</div>
		<div class="content layout">
			<layout1></layout1>
			<layout2></layout2>
			<layout3></layout3>
			<layout4></layout4>
			<layout5></layout5>
			<layout6></layout6>
			<layout7></layout7>
			<layout8></layout8>
			<layout9></layout9>
			<layout10></layout10>
		</div>
		<div class="content behavior">
			<behavior1></behavior1>
			<behavior2></behavior2>
			<behavior3></behavior3>
			<behavior4></behavior4>
			<behavior5></behavior5>
			<behavior6></behavior6>
			<behavior7></behavior7>
			<behavior8></behavior8>
			<behavior9></behavior9>
			<behavior10></behavior10>
			<behavior11></behavior11>
			<behavior12></behavior12>
			<behavior13></behavior13>
			<behavior14></behavior14>
			<behavior15></behavior15>
			<behavior16></behavior16>
			<behavior17></behavior17>
			<behavior18></behavior18>
			<behavior19></behavior19>
			<behavior20></behavior20>
			<behavior21></behavior21>
		</div>
		<div class="content color">
			<color1></color1>
			<color2></color2>
			<color3></color3>
			<color4></color4>
			<color5></color5>
			<color6></color6>
			<color7></color7>
			<color8></color8>
			<!-- <color9></color9> -->
			<color10></color10>
			<color11></color11>
			<color12></color12>
		</div>
		<div class="content figure">
			<figure1></figure1>
			<figure2></figure2>
			<figure3></figure3>
			<figure4></figure4>
			<figure5></figure5>
			<figure6></figure6>
			<figure7></figure7>
			<figure8></figure8>
			<figure9></figure9>
			<!-- <figure10></figure10> -->
			<figure11></figure11>
			<figure12></figure12>
		</div>
		<div class="content component">
			<component1></component1>
			<component2></component2>
			<component3></component3>
			<component4></component4>
			<component5></component5>
			<component6></component6>
			<component7></component7>
			<component8></component8>
			<component9></component9>
			<component10></component10>
			<component11></component11>
			<component12></component12>
			<component13></component13>
			<component14></component14>
			<component15></component15>
			<component16></component16>
			<component17></component17>
			<component18></component18>
			<component19></component19>
			<component20></component20>
			<component21></component21>
			<component22></component22>
			<component23></component23>
			<component24></component24>
			<component25></component25>
			<component26></component26>
			<component27></component27>
			<component28></component28>
			<component29></component29>
			<component30></component30>
			<component31></component31>
			<component32></component32>
			<component33></component33>
			<component34></component34>
		</div>
	</div>
</template>

<style lang="scss">
::-webkit-scrollbar {
	width: 6px;
	height: 6px;
}
::-webkit-scrollbar-track {
	background-color: rgba(#ccc, .3);
}
::-webkit-scrollbar-thumb {
	border-radius: 3px;
	background-color: #ccc;
}
.header {
	overflow: hidden;
	height: 100vh;
	background-color: #282c34;
	h1 {
		margin: 20px 0;
		font-size: 10vmin;
	}
	img {
		display: inline-block;
		height: 10vmin;
		vertical-align: super;
		animation: swing 3s infinite;
	}
	p {
		line-height: 1.5;
		font-size: 1.8vmin;
		color: #fff;
		& + p {
			margin-top: 10px;
		}
	}
	strong {
		display: inline-block;
		margin: 0 3px;
		padding: 0 6px;
		border-radius: 5px;
		line-height: 20px;
		color: #fff;
		&.default {
			background-color: #f66;
		}
		&.react {
			background-color: #61dafb;
		}
		&.vue {
			background-color: #42b983;
		}
	}
	div {
		display: flex;
		margin-top: 20px;
	}
	.gradient {
		background-image: linear-gradient(92deg, #f66 0%, #f90 100%);
		background-clip: text;
		color: #f66;
		animation: hue 5s infinite linear;
		-webkit-text-fill-color: transparent;
	}
}
.bruce {
	overflow: hidden;
	position: relative;
	padding: 50px 0;
	border-bottom: 1px solid #ccc;
	min-height: 300px;
	&::before {
		position: absolute;
		left: 50%;
		top: 0;
		z-index: 99999;
		padding: 0 10px;
		border-radius: 0 0 5px 5px;
		max-width: 300px;
		line-height: 20px;
		color: #fff;
		content: attr(data-title);
		transform: translateX(-50%);
	}
	&::after {
		position: absolute;
		right: 0;
		bottom: 0;
		z-index: 99999;
		padding: 5px 10px;
		border-top-left-radius: 5px;
		background-color: #ccc;
		font-weight: bold;
		font-size: 16px;
		color: #fff;
	}
}
.content {
	overflow: auto;
	transition: all 300ms;
	&.layout .bruce {
		&::before {
			background-color: #f66;
		}
		&::after {
			content: "布局";
		}
	}
	&.behavior .bruce {
		&::before {
			background-color: #66f;
		}
		&::after {
			content: "行为";
		}
	}
	&.color .bruce {
		&::before {
			background-color: #f90;
		}
		&::after {
			content: "颜色";
		}
	}
	&.figure .bruce {
		&::before {
			background-color: #09f;
		}
		&::after {
			content: "图形";
		}
	}
	&.component .bruce {
		&::before {
			background-color: #3c9;
		}
		&::after {
			content: "组件";
		}
	}
}
@keyframes hue {
	from {
		filter: hue-rotate(0);
	}
	to {
		filter: hue-rotate(-360deg);
	}
}
@keyframes swing {
	0%,
	65% {
		transform: rotate(0);
	}
	70% {
		transform: rotate(6deg);
	}
	75% {
		transform: rotate(-6deg);
	}
	80% {
		transform: rotate(6deg);
	}
	85% {
		transform: rotate(-6deg);
	}
	90% {
		transform: rotate(6deg);
	}
	95% {
		transform: rotate(-6deg);
	}
	100% {
		transform: rotate(0);
	}
}
</style>

<script>
import Behavior1 from "./components/behavior/使用@empty监听清空状态";
import Behavior2 from "./components/behavior/使用@focus-within分发冒泡响应";
import Behavior3 from "./components/behavior/使用@hover定制悬浮提示";
import Behavior4 from "./components/behavior/使用@hover控制悬浮边框";
import Behavior5 from "./components/behavior/使用@hover描绘鼠标跟随";
import Behavior6 from "./components/behavior/使用@not()去除无用属性";
import Behavior7 from "./components/behavior/使用@nth-child()选择指定元素";
import Behavior8 from "./components/behavior/使用@valid和@invalid校验表单内容";
import Behavior9 from "./components/behavior/使用+或~美化选项表单";
import Behavior10 from "./components/behavior/使用+或~选择指定元素";
import Behavior11 from "./components/behavior/使用animation-delay保留动画首帧";
import Behavior12 from "./components/behavior/使用attr()控制切换文本";
import Behavior13 from "./components/behavior/使用attr()抓取节点属性";
import Behavior14 from "./components/behavior/使用content提升反爬效果";
import Behavior15 from "./components/behavior/使用max-height切换自动高度";
import Behavior16 from "./components/behavior/使用object-fit规定图像尺寸";
import Behavior17 from "./components/behavior/使用pointer-events禁用事件触发";
import Behavior18 from "./components/behavior/使用position控制吸附位置";
import Behavior19 from "./components/behavior/使用resize拉伸多列分栏";
import Behavior20 from "./components/behavior/使用text-align-last对齐两端文本";
import Behavior21 from "./components/behavior/使用transform模拟视差滚动";

import Color1 from "./components/color/使用@@selection改变选中颜色";
import Color2 from "./components/color/使用@nth-child()描绘信号彩带";
import Color3 from "./components/color/使用box-shadow描绘彩虹色带";
import Color4 from "./components/color/使用filter雕刻高斯模糊";
import Color5 from "./components/color/使用filter开启暗黑模式";
import Color6 from "./components/color/使用filter开启悼念模式";
import Color7 from "./components/color/使用filter描绘彩色阴影";
import Color8 from "./components/color/使用filter描绘动态背景";
// import Color9 from "./components/color/使用filter模拟Instagram滤镜";
import Color10 from "./components/color/使用linear-gradient()控制渐变背景";
import Color11 from "./components/color/使用linear-gradient()控制渐变文本";
import Color12 from "./components/color/使用linear-gradient()控制闪烁文本";

import Component1 from "./components/component/iOS开关按钮";
import Component2 from "./components/component/标签导航";
import Component3 from "./components/component/标签选框";
import Component4 from "./components/component/倒影加载条";
import Component5 from "./components/component/登录注册";
import Component6 from "./components/component/点赞按钮";
import Component7 from "./components/component/迭代计数器";
import Component8 from "./components/component/放大镜";
import Component9 from "./components/component/故障文本";
import Component10 from "./components/component/滚动渐变背景";
import Component11 from "./components/component/滚动指示器";
import Component12 from "./components/component/划线跟随导航";
import Component13 from "./components/component/混沌加载圈";
import Component14 from "./components/component/加载指示器";
import Component15 from "./components/component/立体按钮";
import Component16 from "./components/component/螺纹进度条";
import Component17 from "./components/component/气泡背景墙";
import Component18 from "./components/component/气泡对话框";
import Component19 from "./components/component/三维立方体";
import Component20 from "./components/component/商城打孔票券";
import Component21 from "./components/component/手风琴";
import Component22 from "./components/component/条形加载条";
import Component23 from "./components/component/图像换色器";
import Component24 from "./components/component/心形加载条";
import Component25 from "./components/component/星级评分";
import Component26 from "./components/component/悬浮跟踪按钮";
import Component27 from "./components/component/悬浮视差按钮";
import Component28 from "./components/component/悬浮状态球";
import Component29 from "./components/component/圆角进度条";
import Component30 from "./components/component/粘粘球";
import Component31 from "./components/component/折叠面板";
import Component32 from "./components/component/专栏头像";
import Component33 from "./components/component/自动打字器";
import Component34 from "./components/component/自适应相册";

import Figure1 from "./components/figure/使用box-shadow裁剪聚焦区域";
import Figure2 from "./components/figure/使用box-shadow描绘单侧投影";
import Figure3 from "./components/figure/使用clip-path描绘各种图形";
import Figure4 from "./components/figure/使用clip描绘蛇形边框";
import Figure5 from "./components/figure/使用conic-gradient()描绘彩色饼图";
import Figure6 from "./components/figure/使用linear-gradient()描绘波浪划线";
import Figure7 from "./components/figure/使用linear-gradient()描绘方格背景";
import Figure8 from "./components/figure/使用linear-gradient()描绘方格彩带";
import Figure9 from "./components/figure/使用linear-gradient()描绘网格背景";
// import Figure10 from "./components/figure/使用mask雕刻镂空背景";
import Figure11 from "./components/figure/使用outline描绘内部边框";
import Figure12 from "./components/figure/使用transform描绘动感心形";

import Layout1 from "./components/layout/使用clip-path排版蜂窝布局";
import Layout2 from "./components/layout/使用flexbox排版各种布局";
import Layout3 from "./components/layout/使用float排版环绕文本";
import Layout4 from "./components/layout/使用letter-spacing排版倒序文本";
import Layout5 from "./components/layout/使用margin排版凸显布局";
import Layout6 from "./components/layout/使用overflow-x排版横向列表";
import Layout7 from "./components/layout/使用text-overflow控制溢出文本";
import Layout8 from "./components/layout/使用transform翻转容器内容";
import Layout9 from "./components/layout/使用transform描绘像素边框";
import Layout10 from "./components/layout/使用writing-mode排版竖向文本";

export default {
	name: "app",
	components: {
		// 行为
		Behavior1,
		Behavior2,
		Behavior3,
		Behavior4,
		Behavior5,
		Behavior6,
		Behavior7,
		Behavior8,
		Behavior9,
		Behavior10,
		Behavior11,
		Behavior12,
		Behavior13,
		Behavior14,
		Behavior15,
		Behavior16,
		Behavior17,
		Behavior18,
		Behavior19,
		Behavior20,
		Behavior21,
		// 色彩
		Color1,
		Color2,
		Color3,
		Color4,
		Color5,
		Color6,
		Color7,
		Color8,
		// Color9,
		Color10,
		Color11,
		Color12,
		// 组件
		Component1,
		Component2,
		Component3,
		Component4,
		Component5,
		Component6,
		Component7,
		Component8,
		Component9,
		Component10,
		Component11,
		Component12,
		Component13,
		Component14,
		Component15,
		Component16,
		Component17,
		Component18,
		Component19,
		Component20,
		Component21,
		Component22,
		Component23,
		Component24,
		Component25,
		Component26,
		Component27,
		Component28,
		Component29,
		Component30,
		Component31,
		Component32,
		Component33,
		Component34,
		// 图形
		Figure1,
		Figure2,
		Figure3,
		Figure4,
		Figure5,
		Figure6,
		Figure7,
		Figure8,
		Figure9,
		// Figure10,
		Figure11,
		Figure12,
		// 布局
		Layout1,
		Layout2,
		Layout3,
		Layout4,
		Layout5,
		Layout6,
		Layout7,
		Layout8,
		Layout9,
		Layout10
	},
	data() {
		return {
			count: 0
		};
	},
	mounted() {
		const items = document.getElementsByClassName("bruce") || [];
		this.count = items.length;
	}
};
</script>