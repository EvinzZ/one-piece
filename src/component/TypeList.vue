<template>
    <el-row :gutter="12" style="margin-right: 0">
        <el-col :span="5">
            <el-card shadow="hover">
                <div slot="header" class="clearfix">
                    <span>最新</span>
                    <el-button style="float: right; padding: 3px 0" type="text">更多</el-button>
                </div>
                <div v-for="o in 4" :key="o" class="text item">
                    {{ '列表内容 ' + o }}
                </div>
            </el-card>
        </el-col>
        <el-col :span="5">
            <el-card shadow="hover">
                <div slot="header" class="clearfix">
                    <span>热门</span>
                    <el-button style="float: right; padding: 3px 0" type="text">更多</el-button>
                </div>
                <div v-for="o in 4" :key="o" class="text item">
                    {{ '列表内容 ' + o }}
                </div>
            </el-card>
        </el-col>
        <el-col :span="5">
            <el-card shadow="hover">
                <div slot="header" class="clearfix">
                    <span>月榜</span>
                    <el-button style="float: right; padding: 3px 0" type="text">更多</el-button>
                </div>
                <div v-for="o in 4" :key="o" class="text item">
                    {{ '列表内容 ' + o }}
                </div>
            </el-card>
        </el-col>
        <el-col :span="5">
            <el-card shadow="hover">
                <div slot="header" class="clearfix">
                    <span>周榜</span>
                    <el-button style="float: right; padding: 3px 0" type="text">更多</el-button>
                </div>
                <div v-for="o in 4" :key="o" class="text item">
                    {{ '列表内容 ' + o }}
                </div>
            </el-card>
        </el-col>
        <el-col :span="5">
            <el-card shadow="hover">
                <div slot="header" class="clearfix">
                    <span>日榜</span>
                    <el-button style="float: right; padding: 3px 0" type="text">更多</el-button>
                </div>
                <div v-for="o in 4" :key="o" class="text item">
                    {{ '列表内容 ' + o }}
                </div>
            </el-card>
        </el-col>
    </el-row>
</template>
<style>
.text {
    font-size: 14px;
}

.item {
    margin-bottom: 18px;
}

.clearfix:before,
.clearfix:after {
    display: table;
    content: "";
}

.clearfix:after {
    clear: both
}

.box-card {
    width: 480px;
}
</style>