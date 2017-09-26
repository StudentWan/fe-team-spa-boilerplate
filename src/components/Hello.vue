<template>
    <div class="layout">
        <Menu mode="horizontal" theme="dark" active-name="1">
            <div class="layout-logo"><img class="logo" src="" alt="SafeCode"></div>
            <div class="layout-nav">
                <MenuItem name="1">
                    <Icon type="ios-navigate"></Icon>
                    导航一
                </MenuItem>
                <MenuItem name="2">
                    <Icon type="ios-keypad"></Icon>
                    导航二
                </MenuItem>
                <MenuItem name="3">
                    <Icon type="ios-analytics"></Icon>
                    导航三
                </MenuItem>
                <MenuItem name="4">
                    <Icon type="ios-paper"></Icon>
                    导航四
                </MenuItem>
            </div>
        </Menu>
        <Menu mode="horizontal" active-name="1">
            <div class="layout-assistant">
                <MenuItem name="1">二级导航</MenuItem>
                <MenuItem name="2">二级导航</MenuItem>
                <MenuItem name="3">二级导航</MenuItem>
            </div>
        </Menu>
        <div class="layout-breadcrumb">
            <Breadcrumb>
                <BreadcrumbItem href="#">首页</BreadcrumbItem>
                <BreadcrumbItem href="#">应用中心</BreadcrumbItem>
                <BreadcrumbItem>某应用</BreadcrumbItem>
            </Breadcrumb>
        </div>
        <div class="layout-content">
            内容区域
        </div>
        <div class="layout-copy">
            2011-2016 &copy; TalkingData
        </div>
    </div>
</template>
<script>
    /**
     * @author {benyuwan@gmail.com}
     * @file 欢迎页面
     */
    export default {}
</script>
<style lang="scss" scoped>
    .layout {
        height: 100%;
        border: 1px solid #d7dde4;
        background: #f5f7f9;
    }

    .layout-logo {
        width: 100px;
        height: 30px;
        background: #5b6270;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
        .logo {
            max-height: 100%;
            position: relative;
            bottom: 15px;
            color: #58b857;
            font-weight: 700;
        }
    }

    .layout-nav {
        width: 420px;
        margin: 0 auto;
    }

    .layout-assistant {
        width: 300px;
        margin: 0 auto;
        height: inherit;
    }

    .layout-breadcrumb {
        padding: 10px 15px 0;
    }

    .layout-content {
        min-height: 400px;
        margin: 15px;
        overflow: hidden;
        background: #fff;
        border-radius: 4px;
        color: $pink;
    }

    .layout-content-main {
        padding: 10px;
    }

    .layout-copy {
        position: fixed;
        left: 50%;
        bottom: 0;
        transform: translateX(-50%);
        text-align: center;
        padding: 10px 0 20px;
        color: #9ea7b4;
    }
</style>
