<template>
	<div class="home">
		<el-container>
			<el-aside width="200px">
				<el-menu :router=true class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
					<el-submenu>
						<template slot="title">
							<i class="el-icon-menu"></i>
							<span>首页</span>
						</template>
					</el-submenu>
				</el-menu>
				<el-menu :router=true class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
					<el-submenu>
						<template slot="title">
							<i class="el-icon-folder"></i>
							<span>数据管理</span>
						</template>
						<el-menu-item index="/home/user1">
							<span>用户列表</span>
						</el-menu-item>
						<el-menu-item index="/home/user2">
							<span>商家列表</span>
						</el-menu-item>
						<el-menu-item index="/home/user3">
							<span>食品列表</span>
						</el-menu-item>
						<el-menu-item index="/home/user3">
							<span>订单列表</span>
						</el-menu-item>
						<el-menu-item index="/home/user3">
							<span>管理员列表</span>
						</el-menu-item>
					</el-submenu>
				</el-menu>
				<el-menu :router=true class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
					<el-submenu>
						<template slot="title">
							<i class="el-icon-plus"></i>
							<span>添加数据</span>
						</template>
						<el-menu-item index="/home/user1">
							<span>添加商铺</span>
						</el-menu-item>
						<el-menu-item index="/home/user2">
							<span>添加商品</span>
						</el-menu-item>
					</el-submenu>
				</el-menu>
				<el-menu :router=true class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
					<el-submenu>
						<template slot="title">
							<i class="el-icon-orange"></i>
							<span>图表</span>
						</template>
						<el-menu-item index="/home/user1">
							<span>用户分布</span>
						</el-menu-item>
					</el-submenu>
				</el-menu>
			</el-aside>
			<el-container>
				<el-header>首页</el-header>
				<el-main>Main</el-main>
			</el-container>
		</el-container>
	</div>
</template>

<script>
	export default {
		name: "Home"
	}
</script>

<style scoped>
	.home {
		height: 100%;
	}
	
	.el-menu-admin:not(.el-menu--collapse) {
		width: 200px;
		min-height: 400px;
	}
	
	.el-container {
		height: 100%;
	}
	
	.el-aside {
		background-color: #545c64;
	}
	
	.el-header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		background-color: rgb(239, 242, 247);
	}
	
	.logo {
		height: 60px;
		background: url(../assets/logo.png);
		background-size: cover;
		background-color: #989898;
	}
	
	.toggle-btn {
		font-size: 36px;
		color: #989898;
		cursor: pointer;
		line-height: 60px;
	}
	
	.system-title {
		font-size: 28px;
		color: white;
	}
	
	.welcome,
	{
		color: white;
	}
</style>